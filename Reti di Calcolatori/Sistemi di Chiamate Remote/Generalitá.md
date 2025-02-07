Internet a causa della sua filosofia di limitazione dei costi utilizza una semantica dei servizi **may-be** o **best effort**, cioè ogni azione è effettuata una singola volta senza preoccupazione della qualità.
#### Semantiche di ritrasmissione
Per aumentare il livello del *QoS* esistono diverse semantiche di ritrasmissione:
* **At least once**: Il client in caso di errore di trasmissione/conferma del messaggio rimanda il messaggio al server che a questo punto riesegue l'operazione e manda la conferma.
* **At most once**: Il client in caso di errore di trasmissione/conferma del messaggio rimanda come nella semantica **at least once**, ma in questo caso il server si accorge della ripetizione e non riesegue l'operazione, ma manda solo il risultato.
* **Exactly once**: In questo caso o il messaggio è arrivato e la risposta tornata, oppure nessuna azione viene eseguita (con opportuno rollback), l'operazione è quindi atomica ed eseguita solo se non ci sono stati errori.

Ognuna di queste decisioni di implementazione hanno i loro pregi e difetti, in generale semantiche at most/exactly once sono più pesanti da un livello implementativo, ma garantiscono il miglior *QoS*. Per esempio TCP utilizza una semantica *at most once* con ritrasmissione dei pacchetti persi
# RPC
**Remote Procedure Call** è un estensione del normale meccanismo di chiamate a procedure locale che si occupa di chiamate a procedure su macchine differenti.
* Il cliente è **sincrono bloccante**.
* I cliente e servitore hanno lifetime indipendenti.
* Sono possibili errori di rete e su nodi diversi da quello del chiamante.

RPC fornisce inoltre i seguenti servizi necessari all'operazione: 
* Controllo dei tipi di ingresso uscita.
* Marshalling/unmarshalling dei parametri di ingresso e uscita.
* Utilizzo trasparente per il cliente, come se la procedura fosse locale.
* Binding dinamico dei nomi dei servitori.

In caso di errore e/o timeout il cliente può scegliere se ritrasmettere (operazioni **idempotenti**, semantica **at least once**) o riportare un eccezione al cliente.
Dalla parte del servitore invece bisogna gestire il crash del client e i figli orfani, con eliminazione **istantanea**, oppure automatica dopo un **timeout**.

### RPC - Stub
Una prima implementazione più semplice utilizza una funzione 
``` c
void* callrpc(nome_remoto, id_proc, args)
```
che si occupa della chiamata RPC in modo non trasparente, invece altre implementazioni più trasparenti fanno utilizzo di **stub**, forniti dai servizi RPC e generati automaticamente, che chiamati provvedono loro alla chiamata remota nascondendo dettagli implementativi.
In maniera analoga un secondo stub dalla parte del serve si occupa della trasparenza lato server, in modo che la procedura del server possa essere implementata come se chiamata localmente.
Gli **stub** occupano quindi di:
* Marshalling dati outbound
* Unmarshalling dati inbound
* Controllo risultato ed eventuale ritrasmissione.

### RPC - Passaggio dei Parametri
I dati essendo su macchine diverse non possono essere passati normalmente:
* La maggior parte delle implementazioni passa i parametri per valore effettuando la **serializzazione** (marshalling) e **deserializzazione** (unmarshalling).
* Alcune implementazioni come ad esempio RMI implementano il passaggio per **riferimento remoto**.

I dati in uscita devono a questo punto avere un lifetime sufficientemente esteso per garantire il corretto trasferimento verso l'altra macchina e deve essere aggiornato in caso di modifica remota.

### RPC - Interface Definition Language
Uno dei problemi più importanti è la condivisione del contratto di funzionamento tra client/server e la creazione degli [[Generalitá#RPC - Stub|stub]], al servizio di questi due problemi intervengono dei linguaggi appositi chiamati IDL che:
* Definiscono in maniera univoca i servizi disponibili in un server.
* Definiscono i tipi di dati utilizzati nei contratti di esecuzione dei servizi.

Purtroppo esistono diverse implementazioni di questi linguaggi, che porta ad una bassa standardizzazione pratica.

### RPC - Binding dei servizi
Il binding si occupa di trovare la locazione fisica di un servizio dato un nome logico di esso.
* Nel **binding statico** la locazione del servizio è hardcoded nel programma, soluzione meno costosa ma non flessibile.
* Nel **binding dinamico** si utilizza un servizio esterno che si occupa di trovare la locazione fisica da un nome logico, soluzione complessa ma più estensibile.

Il binding dinamico può essere effettuato con il protocollo di **bidding** in broadcast, oppure con un sistema di nomi esterno.