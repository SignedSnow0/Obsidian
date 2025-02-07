OSI è uno standard di comunicazione tra sistemi eterogenei, si pone come obbiettivo quello di controllare, coordinare e monitorare sistemi interconnessi senza limiti di località e di coresidenza.
OSI è organizzato in 7 livelli:
* Fisico, data link, network nella parte fisica.
* Trasporto come intermediario tra parte fisica e logica.
* Sessione, presentazione, applicazione nella parte logica.

Ogni livello prevede una suite di servizi utilizzati dal protocollo superiore attraverso un'interfaccia comune. Ogni livello è composto da due parti
* Un **protocollo** da realizzare definendo lo standard di quel livello utilizzato per fornire un servizio.
* Un **servizio** da richiedere in modo verticale tramite l'interfaccia standard.

### Comunicazione tra livelli
Due applicazioni per comunicare devono poter identificare il corrispondente dall'altro lato per ogni livello dello stack. Ogni livello OSI definisce almeno un **Service Access Point** al livello superiore per l'utilizzo del servizio fornito, questo SAP deve avere un nome unico per poterlo identificare, allora per identificare un'entità remota bisogna nominare tutti i SAP dal livello 1 al 7.
Nella pratica un'entità è identificata solamente fino al nome di livello 3 in su, perciò non sono necessari nomi del livello data link e fisico (tutti i nomi dei protocolli end to end).
### Primitive e forme
In maniera generale, i servizi di pari livelli comunicano tramite quattro categorie di richieste non obbligatorie (tutte presenti nel caso di servizio sincrono):
* Request: l'utente richiede un servizio.
* Indication: il server segnala che è stato richiesto un servizio.
* Response: il client specifica il servizio da effettuare.
* Confirm: il server risponde con i dati prodotti dal servizio.
## Livello di Rete
Il livello di rete è uno dei livelli fisici, tiene conto quindi dei nodi intermedi ai due host finali. Il livello si occupa delle realizzazioni di routing tra diverse reti e definisce il sistema di nomi delle entità. Il livello si occupa di:
* Indirizzamento (nomi IP).
* Controllo di flusso tra nodi.
* Controllo di congestione del sistema.
## Livello di trasporto
Il trasporto è il primo livello end to end, inoltre il livello di trasporto è multiplo in una singola macchina, perciò un singolo SAP di rete è collegato a molteplici SAP di trasporto (più porte e un solo IP).
* Il livello di trasporto ha la capacità di spezzare un messaggio per essere trasportato e ricomporlo al nodo finale.
* Il livello di trasporto ha la capacità di multiplexing e demultiplexing verso il layer di rete.
* In modalità con connessione il livello ha l'onere di creare e terminare la connessione.
* Il trasferimento dei dati è diviso in normali e privilegiati (expedited).
## Livello di Sessione
Il lavoro del livello di sessione è quello del supporto al **dialogo**, definito come una sequenza di messaggi componenti di un oggetto di dimensione variabile.
Il dialogo può:
* Essere bidirezionale.
* Molteplice per una singola applicazione.
* Impegnare risorse.
* Avere garanzie di affidabilità.

Oltre al livello di trasporto il livello di sessione si occupa di autorizzazione della comunicazione e creazione di punti di sincronizzazione (checkpoint), il numero di primitive è ampio (58 rispetto alle 4 del trasporto), sono divise in tre macrocategorie:
* Azioni di **controllo** (autorizzazione, sincronizzazione).
* Divisione del dialogo in **attività** e azioni su di essere.
* Notifica di **eccezioni**.

I punti di sincronizzazione sono fondamentali per esempio nella comunicazione di grosse quantità di dati dove per esempio in caso di errore si vuole cercare di non dove ritrasmettere tutte le informazioni.
* I punti di sincronizzazione **minori** sono punti per il quale il ricevente deve inviare conferma al mittente anche se il mittente continua con la trasmissione.
* I punti di sincronizzazione **maggiori** invece richiedono l'attesa del mittente della ricezione della conferma (sincrono bloccante).

In caso di errore i punti di sincronizzazione sono utilizzati per il recupero della comunicazione: con primitiva confirm in caso di punto maggiore e con sliding window (di dimensione negoziabile) in caso di punti minori.
Infine il livello di sessione si occupa di autenticazione attraverso il meccanismo dei token, oggetti astratti passati nella comunicazione e creati nella creazione della connessione, i token sono distinti in base alle operazioni da eseguire:
* Data token per spedizione di dati.
* Release token per chiudere la connessione.
* Synchronize minor/major token per la creazione di punti di sincronizzazione.
## Livello di Presentazione
## Livello Applicativo