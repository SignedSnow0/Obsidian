I **sistemi distribuiti** sono particolari architetture di calcolatori diversi che collaborano per ottenere un modello di esecuzione più esteso, nonostante la maggiore complessità architetturale rispetto a un modello a macchina singola, apportano i seguenti vantaggi fondamentali nel mondo moderno:
* Accesso a **risorse remote** da dovunque.
* Condivisione di **informazioni** da remoto.

le architetture distribuite sono collegate a diverse difficoltà concettuali
* Concorrenza fra processi che risiedono su macchine diverse.
* Assenza di metodi di sincronizzazione globale.
* Diversi punti di collegamento, ognuno con i suoi potenziali errori.

inoltre le architetture distribuite devono avere alcune proprietà fondamentali
* Trasparenza dei nodi fisici.
* Dinamicità dei sistemi.
* Qualità del servizio.
## Standard e definizioni
Ogni tipo di comunicazione può essere implementata con uno dei seguenti tipi di implementazione in maniera indipendente e completa in ciascuno dei casi:
* Scambio di Messaggi
* Cliente - Servitore

Ci sono altre definizioni di comunicazione più o meno utilizzate in uno dei due tipi di comunicazione
* Sincrono/Asincrono: il nodo decide o meno di aspettare risposta (se è presente).
* Bloccante/Non bloccante: il nodo aspetta la risposta prima di continuare.
* Simmetrico/Asimmetrico: il nodo conosce o meno la presenza degli altri nodi.

Nel corso approfondiremo il protocollo **cliente/servitore sincrono bloccante asimmetrico** diventato standard *de facto* nella maggior parte delle applicazioni.
Inoltre il **binding** è **dinamico**, cioè la locazione fisica del server è ottenuta a runtime, spesso attraverso l'utilizzo di servizi terzi come i **sistemi di nomi**.
## Specifiche dell modello cliente/servitore
Il cliente tipicamente lavora in modo sincrono e bloccante, ma in caso di errore la risposta potrebbe non arrivare mai, per questi casi è di solito definito un tempo massimo oltre il quale il client presume ci sia stato un errore, il tempo di **timeout**.
Le azioni da prendere a seguito di un timeout sono differenti e comportano le proprie conseguenze, se per esempio la richiesta era già arrivata, una nuova richiesta potrebbe comportare errori logici.

Il servitore è in generale più complesso del cliente per il semplice fatto che deve gestire molte più richieste per secondo del cliente.
* In generale il servitore è un processo demone, cioè che non termina mai, per poter rispondere alle richieste in qualsiasi momento.
* Il servitore in genere deve accedere a dati persistenti, risolvere problemi di validità di essi e autenticare i client.
* Inoltre il servitore deve rispondere a molte richieste alla volta, è quindi di solito implementato con diversi gradi di parallelismo, con problemi associati.
* Soprattutto il client, ma anche il server deve essere progettato come un filtro, processo collegato ad uno stream di input che viene completamente consumato per la corretta esecuzione.
* Il client e server comunicano secondo un protocollo accordato.
## Modelli di comunicazione
Le prime suddivisioni dei modelli di comunicazione parlano di come i messaggi sono distribuiti tra client e server.
* **Polling** o **pull**: il modello di polling è uno dei modelli di comunicazione più semplici, dove il client chiede periodicamente aggiornamenti al server. Questo metodo è altamente inefficiente e idealmente molte delle risposte sono inutili in quanto il dato non è stato modificato.
* **Push**: il modello a push è più sofisticato è consiste in una prima fase dove un cliente che desidera ottenere aggiornamenti si **sottoscrive** ad un servizio del server, che poi in caso di aggiornamenti manda l'informazione al client in ascolto.
* Esistono altri modelli a **delegazione** per interazioni non bloccanti dove la risposta è delegata a entità terze come proxy, spesso usate in modelli a scambio di messaggi come la mail.

La seconda suddivisione è in base al tipo di canale creato per la comunicazione.
* I modelli **connection oriented** stabiliscono durante una fase di discovery un canale di comunicazione virtuale impegnando una serie di nodi fra il cliente e il servitore (OSI).
* I modelli **connectionless** invece decidono il percorso di comunicazione momento per momento a secondo della situazione attuale del pacchetto (IP).

In generale i modelli connection oriented producono una migliore QoS, mentre i modelli connectionless producendo una QoS peggiore sono più resistenti a errori nel circuito di trasporto e sono quelli implementati nella pratica con il protocollo IP, nonostante ciò si cercano comunque astrazioni alla connessione nel livello di trasporto con TCP.