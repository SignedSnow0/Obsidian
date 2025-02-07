## Indirizzi IP in Unix
Unix supporta indirizzi per diversi sistemi di nomi oltre all'IP, perciò oltre alla struttura generica *sockaddr* si specifica una struttura apposita per i protocolli internet
``` c
/* sys/socket.h */
struct sockaddr {
	short int sa_family;
	char sa_data[14];
};

/* netinet/in.h */
struct in_addr {
	long int s_addr;	
};

struct sockaddr_in {
	short int sin_family; /* Sempre AF_INET */
	short int sin_port;
	struct in_addr sin_addr;
	
	char sin_zero[8] _reserverd;
};
```
gli indirizzi IP sono ottenuti con query DNS attraverso la funzione *gethostbyname*
``` c
/* netdb.h */
struct hostent {
	char* h_name; /* nome dell'host */
	char** h_aliases; /* lista degli aliases */
	int h_addrtype; /* tipo di indirizzo */
	int h_length; /* lunghezza dell'indirizzo */
	char** h_addr_list; /* lista di indirizzi */
}


struct hostent* gethostbyname(const char* name);
```
in questo caso *h_addr_list[0]* corrisponde all'indirizzo ip principale da inserire in *sin_addr.s_addr*, per i server è utile settare *s_addr=INADDR_ANY* che rappresenta tutti gli indirizzi locali.
Esiste una seconda funzione meno utilizzata per ottenere la porta da un nome logico
``` c
/* netdb.h */
struct servent* getservbyname(const char* name, int proto);
```
Per la creazione della socket vera e propria si utilizza la syscall *socket*
``` c
/* sys/socket.h */
int socket(int domain, int type, int proto);
```
* Domain rappresenta il dominio (unix, internet, ecc).
* Type specifica la connessione (datagram, stream, ecc).
* Proto identifica eventuali protocolli (non utilizzato in internet).
* Il valore restituito è un descriptor alla socket creata.

Una volta creata la socket bisogna collegarla ad un indirizzo 
``` c
int bind(int socket, struct sockaddr* name, int name_length);
```
* Il valore restituito è un eventuale codice di errore.
## Socket Datagram
Una volta creata una socket di tipo *SOCK_DGRAM* e bindata su un indirizzo è possibile comunicare attraverso le primitive
``` c
int sendto(int sock, char* msg, int len, int flags, struct sockaddr* to, int tolen);
int recvfrom(int sock, char* msg, int len, int flags, struct sockaddr* from, int fromlen);
```
* sock indica la socket locale da utilizzare per la comunicazione.
* msg è un buffer nel quale i dati sono locati.
* len indica la dimensione del buffer.
* flags sono flag di comportamento (MSG_PEEK non consuma il dato).
* to/from rappresenta l'indirizzo dell'altra macchina.
* to/from len india la lunghezza di to/from.

La coda dei datagrammi che aspettano di essere processati è modificabile con l'opzione *SO_RCVBUF/SO_SENDBUF*, essendo UDP protocollo best effort i datagrammi che non entrano nella coda sono scartati senza notifica.
## Socket Stream
Grazie all'uniformità dei sistemi unix la lettura e scrittura dalle socket stream utilizza le stesse primitive dei files
``` c
int read(int fd, char* buf, int length);
int write(int fd, char* buf, int length);
```
il comportamento è comunque differente, per esempio la read è ora bloccante finchè non arrivano dei dati in entrata, mentre  per un normale file restituirebbe 0 alla fine del file, nelle socket 0 è restituito solamente se la connessione viene chiusa.
Dopo la bind le socket stream richiedono un ulteriore call per il client e per il server
``` c
int connect(int sock, struct sockaddr* addr, int addlen);
int listen(int sock, int backlog)
int accept(int sock, struct sockaddr* addr, int addrlen);
```
* Il client effettua la *connect* che si occupa della creazione del circuito virtuale verso il server.
* Il server effettua prima la listen e poi chiama la *accept* che blocca il processo fino all'arrivo di un client rappresentato da un socket descriptor restituito e indirizzo come parametro di output. 

Alla fine del processo, è opportuno liberare le risorse occupate tramite la primitiva close
``` c
int close(int fd);
```
dopo la chiamata, il processo è incapace di ricevere/trasmettere dati, mentre l'altro processo alla lettura riceverà un EOF, mentre le scritture genereranno un errore di pipe broken, inoltro nonostante la chiamata la driver inoltra comunque i dati nel suo buffer per tempo indeterminato (a meno che non sia specificato nella SO_LINGER).
Esistono altre primitive in grado di chiudere un solo lato della comunicazione 
``` c
int shutdown(int sock, int how) /*how=SHUT_RD SHUT_WR*/
```

## Servitore con più endpoint: Select
La *select* è una primitiva unix che permette di bloccare il processo finchè uno dei descriuptor specificati non è pronto per un azione
``` c
int select(int nfds, int* readfds, int* writefds, int exceptfds, struct timeval* timeout);
```
La select prevede tre liste di descriptor di lunghezza massima *nfds*
* Eventi di lettura (recvfrom, read, accept).
* Eventi di scrittura (sendto, write, connect).
* Eccezioni (close, shutdown).

allo sblocco della funzione il sistema operativo ha impostato un flag per ogni descriptor con azione disponibile, cosicchè il processo può avanzare il funzionamento senza tempi di attesa, inoltre la primitiva prevede un tempo massimo di attesa.
Le tre maschere sono un array di bit pari al massimo file descriptor contenuto nelle tre liste, in ingresso i bit indicano se il descriptor deve essere considerato per l'azione in cui è contenuto, mentre in uscita indica o meno se il descriptor è disponibile per l'azione.
Per facilitare le operazioni sulle maschere sono disponibili una serie di macro:
``` c
FD_SET(int fd, fd_set &fdset); /* aggiunge un descriptor in un set */
FD_CLR(int fd, fd_set &fdset); /* rimuove un descriptor dal set */
FD_ISSET(int fd, fd_set, &fdset); /* controlla che il descriptor sia settato nel set */
FD_ZERO(fd_set &fdset); /* svuota un set */
```