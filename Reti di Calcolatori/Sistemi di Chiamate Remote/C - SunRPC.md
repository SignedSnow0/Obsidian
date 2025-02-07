L'obiettivo di RPC di Sun è quello di permettere la chiamata remota di servizi in maniera trasparente, comunicando quindi dal livello **applicativo**, l'infrastruttura di Sun fornisce quindi i seguenti servizi:
* Scambio di messaggi di chiamata e risposta dei servizi e identificazione della procedura richiesta.
* Gestione della rappresentazione di dati eterogenea.
* Gestione errori di comunicazione o esecuzione.

SunRPC lavora su un astrazione **client/server** con semantica **at least once**, chiamate **sincrone bloccanti** e servitore **sequenziale**.
* I servizi disponibili sono identificati con una tripla **programma**, **versione**, **procedura**, il protocollo di comunicazione (TCP/UDP) è lasciato a discrezione dell'utente con UDP di default.
* Le procedure possono avere un singolo parametro di ingresso e un singolo parametro di uscita.
* Il formato dei dati e le procedure disponibili sono specificate in un file **XDR** usato per la creazione degli **stub**.

``` c
program EXAMPLEPROG {
	version EXAMPLEVERS {
		int EXAMPLEPROC(string) = 1;
	} = 1;
} = 0x20000001;
```

## SunRPC - PortMapper
Il portmapper è un servizio fornito da RPC utilizzato per il binding dinamico dei servizi con la loro locazione fisica.
* Le entry del portmapper sono caratterizzate dalla coppia *{program, version, proto}* e *{port}* in una linked list, manca il **numero di procedura** che è trovato a **tempo di invocazione** e non di registrazione.
* La primitiva **svc_run** è utilizzata dal portmapper dopo la per mettere in esecuzione infinita il processo che deve fornire i servizi al client.
* La porta del servizio è registrata nel **gestore di trasporto** del cliente.
* Ogni servizio registrato è associato a due **gestori di trasporto** del server, uno per TCP, uno per UDP, con la stessa porta creata dal numero di programma e di versione.
* Il portmapper è situato sulla porta 111 con UDP di default, permette inserimento/eliminazione di servizi, lista di tutti i servizi e ottenimento nome fisico di un servizio.
* Le richieste inoltrate contengono informazioni di **autenticazione** del client.
## SunRPC - eXternal Data Representation
XDR è la soluzione della Sun ai problemi del livello di presentazione, consiste in un linguaggio di definizione per specificare:
* **Tipi di dati** utilizzati nelle comunicazioni.
* **Firma** delle procedure di un programma e versione.
* **Marshalling/Unmarshalling** dei dati tra client e server attraverso gli **stub** generati.
* XDR fornisce tipi atomici, tipi standard (con costruttori predefiniti) e tipi definibili dall'utente.
* Tutte le funzioni di conversione restituiscono in booleano che indica il successo della conversione.
## SunRPC - Gestore di trasporto
Il gestore di trasporto è una struttura dati specifica per il protocollo di trasporto che contiene le informazioni necessarie per il funzionamento di RPC, contiene:
* Socket e porta del S.O.
* PFN a funzioni di supporto (ricezione/invio richieste, creazione/distruzione memoria dei dati trasportati).
* Indirizzo remoto e lunghezza associata.

Il client invece contiene informazioni invece riguardo:
* Autenticazione.
* Chiamata da invocare.
* Gestione errori e memoria di ingresso/uscita.
* Annullamento chiamata.
* Timeout per ritrasmissione in caso di gestore UDP.
# Approfondimenti
