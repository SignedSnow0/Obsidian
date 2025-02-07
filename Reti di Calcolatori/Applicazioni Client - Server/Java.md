In Java abbiamo disponibile le **socket** per realizzare applicazioni client/server con strumenti standard. Il primo problema delle socket è che prevedono comunicazione [[Reti di Calcolatori/Applicazioni Client - Server/Generalità#Standard e definizioni|asincrona]], perciò dobbiamo implementare a mano la sincronia:
* Il cliente all'invio di una richiesta attende subito dopo la ricezione di una risposta.
* Il server manda una risposta per ogni richiesta in entrata.
* L'ordine di invio di richieste/risposte deve essere definito dall'ingegnere in un protocollo.

Inoltre nel modello classico client/server il cliente deve conoscere il servitore, il nome fisico della socket è dato dalla coppia *IP, porta*, che identificano il nome della macchina e del processo rispettivamente. Sarebbe però opportuno ottenere questi nomi in maniera dinamica, per questi scopi si utilizzano [[Sistemi di Nomi|sistemi di nomi]].

In Java esistono due tipi di socket:
* TCP per una connessione connection oriented attraverso le **stream**.
* UDP per una connessione connectionless attraverso i **datagram**.
## Indirizzi IP: InetAddress
La classe *InetAddress* è una classe di supporto agli indirizzi IP, non ha costruttori ma è ottenibile attraverso factory:
``` java
static InetAddress InetAddress.getByName(String hostname)
static InetAddress[] InetAddress.getAllByName(String hostname);
static InetAddress InetAddress.getLocalHost();
```
questi metodi ottengono un indirizzo IP tramite risoluzione [[Sistemi di Nomi#Domain Name System|DNS]], possono lanciare *UnknownHostException* in caso il nome non abbia corrispondenze.

## Socket Datagram
Le socket datagram permettono lo scambio di messaggi senza la creazione di una connessione (overhead minore, QoS peggiore), la classe che le rappresenta è la *DatagramSocket*
``` java
DatagramSocket(InetAddress localAddress, int localPort)
```
il costruttore crea una nuova socket e ne effettua il binding all'endpoint specificato.
Lo scambio di messaggi è effettuato tramite i due metodi
``` java
void DatagramSocket.send(DatagramPacket p);
void DatagramSocket.receive(DatagramPacket p);
```
la *send* implica solamente che i dati sono stati passati al kernel per il processamento, invece la receive si mette in attesa bloccando il programma fino all'arrivo di un pacchetto.
I dati sono "impacchettati" in una struttura di supporto chiamata *DatagramPacket*, la classe oltre a contenere i dati passati  contiene informazioni riguardo al mittente (in caso di ricezione), come IP e porta.
``` java
DatagramPacket(byte[] buf, InetAddress address, int port);
```
con relativi getters e setters.
Una caso particolare di comunicazione datagram fa utilizzo di indirizzi IP di classe D per la comunicazione multicast:
``` java
MulticastSocket(int localPort);

void MulticastSocket.joinGroup(InetAddress group);
void MulticastSocket.leaveGroup(InetAddress group);
``` 

le socket permettono la specifica di opzioni aper modificarne il comportamento:
``` java
void Socket.SetSoTimeout(int timeoutMillis);
void Socket.SetSendBufferSize(int size);
void Socket.SetReceiveBufferSize(int size);
void Socket.SetReuseAddress();
```
## Socket Stream
Le socket stream consentono lo scambio di informazioni attraverso un canale di comunicazione creato appositamente , la classe che le rappresenta è
* *Socket* per il client.
* *ServerSocket* per il server.

La connessione è definita dalla quadrupla dei due endpoint: *ipClient, portaClient, ipServer, portaServer*, grazie al protocollo TCP si hanno alcune proprietà
* Semantica [[Generalitá#Semantiche di ritrasmissione|at most once]].
* Comunicazione full duplex.
* Ricezione ordinata.

Java astrae molti dettagli nelle sue API semplificando il lavoro del programmatore, per esempio il costruttore della *Socket*
``` java
Socket(InetAddress remoteAddress, int remotePort);
```
crea la socket, effettua il bind su un indirizzo locale e si connette con la socket del server, tutto in tempo di costruzione.
La suite java fornisce inoltre una serie di astrazioni su flussi di dati, con il wrapper pattern possiamo creare un flusso di alto livello al di sopra  delle stream di input/output di una socket
``` java
InputStream Socket.getInputStream();
OutputStream Socket.getOutputStream();
```

``` java
DataInputStream(InputStream stream);
DataOutputStream(OutputStream stream);

void DataInputStream.writeUTF(String s);
void DataInputStream.writeChar(char c);
void DataInputStream.writeInt(int i);
```
Le socket impegnano risorse di sistema, perciò è importante rilasciarle appena il processo non ne ha più bisogno, le socket implementano l'interfaccia *AutoCloseable* che rilascia le risorse alla distruzione dell'oggetto secondo il pattern *raii*, se invece si vogliono liberare le risorse esplicitamente la *socket* fornisce i seguenti metodi
``` java
synchronized void Socket.close();
void Socket.shutdownInput();
void Socket.shutdownOutput();
```
la *close* chiude entrambi i canali di comunicazione, mentre è possibile chiudere solamente uno dei due lati come previsto dal protocollo TCP.

Il server invece utilizza la *ServerSocket*
``` java
ServerSocket(int localPort);

Socket ServerSocket.accept();
```

il compito della *ServerSocket* è solamente quello di mettersi in attesa di un client, una volta effettuata la connessione la *accet* restituisce una *Socket* attraverso la quale avviene la vera e propria comunicazione.