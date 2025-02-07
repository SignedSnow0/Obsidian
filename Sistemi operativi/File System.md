Il file system è la parte del sistema operativo che si occupa della scrittura e lettura di dati nella memoria di massa, i dati sono strutturati in tre componenti
1. File
2. Cartelle (insieme di file organizzati logicamente)
3. Partizioni (insieme di file nello stesso dispositivo fisico)
---
## Componenti del file system
> [!definition] File
> Un file è individuato da un nome che il sistema operativo utilizza per trovare la sua posizione fisica, inoltre è dotato di diversi metadati contenuti nel suo **file descriptor**, fra i quali:
> * Tipo (come interpretare i dati contenuti)
> * Indirizzo (posizione dei dati nella memoria di massa)
> * Dimensione (numero di byte allocati per il file)
> * Data e ora (dell'ultima modifica)

Inoltre se il sistema operativo permette l'utilizzo da più utenti vengono memorizzati anche
* Utente proprietario
* Diritti di accesso per tutti gli altri utenti

Le operazioni eseguibili sui file sono:
* Creazione / Eliminazione
* Lettura
* Scrittura

> [!definition] Cartelle
> Le cartelle sono un modo per organizzare un gruppo di file in una struttura gerarchica, sono possibili le seguenti operazioni:
> * Creazione / Cancellazione di cartelle
> * Aggiunta / Rimozione di file
> * Elenco dei file contenuti

I sistemi operativi moderni implementano per le cartelle una strutture a grafo aciclico, in poche parole permettono la creazione di cartelle innestate ad infiniti livelli, e permettono di accedere ad uno stesso file da più nomi logici diversi (symlinks o collegamenti).

> [!definition] Partizione
> La partizione rappresenta un singolo dispositivo di memorizzazione di massa, però nei sistemi operativi moderni è possibile dividere un dispositivo fisico in più partizioni logiche.

Di solito prima di poter accedere al file system della partizione è necessario eseguire il *mounting* di essa che può richiedere permessi di amministratore.

---
## Struttura fisica
> [!definition] Blocco
> Un blocco è una sezione di dimensione fissa utilizzata nelle operazioni di lettura/scrittura sul dispositivo fisico.

> [!definition] Record logico
> Un record logico è un'unità di trasferimento utilizzata dai programmi di dimensione variabile, costituita da più blocchi.

Il sistema operativo ha quindi il compito di mantenere la corrispondenza fra blocchi e record.
Per accedere a questi dati sono utilizzati 3 algoritmi diversi:
* Accesso sequenziale: Il file è composto da una sequenza contigua di record logici, l'i/o pointer indica il record attuale e ci si può spostare solo di 1 unità alla volta.
* Accesso diretto: Il file è un insieme di record logici associati ad un indice, per accedere ad uno di questi record basta indicarne l'indice.
* Accesso a indice: Ogni file è associato ad una valore chiamato indice o chiave, allora il record logico sarà il risultato della ricerca per valore.

I blocchi invece sono allocati in memoria fisica utilizzando simili algoritmi:
* Allocazione contigua: analoga all'accesso sequenziale.
* Allocazione a linked list.
* FileAllocationTable: è il metodo utilizzato dai sistemi windows, consiste nella creazione di una tabella all'inizio della partizione che contiene il primo blocco del file, continuando poi con una linked list.
* Allocazione a indice: simile a FAT, ma tutti i blocchi sono contenuti nella tabella.