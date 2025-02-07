> [!definition] Monitor
> Il monitor è una struttura di sincronizzazione tale che:
> * Le operazioni eseguite sui dati sono mutualmente esclusive fra di loro.
> * I dati sono accessibili solo attraverso le operazioni del monitor.

Nella pratica il monitor è un'evoluzione di un [[Semaphore - Java|semaphore]] che permette
* L'accesso mutualmente esclusivo ai dati.
* Un ordine di accesso personalizzabile.

L'accesso esclusivo è garantito attraverso un *lock*, mentre l'ordine personalizzabile è implementato con una *condition*, perciò:
1. L'accesso dal monitor alla risorsa è condizionata dal lock (*entry queue*).
2. L'accesso dal processo al monitor dipende dalla condition (*condition queue*).
![[Monitor.png]]
La condition ha due metodi principali:
* *await()* sospende il processo chiamante e lo inserisce nella *queue*, una volta soddisfatta il processo prende possesso esclusivo della risorsa.
* *signal()* riattiva il primo processo nella *queue*.

Per definizione un solo processo può eseguire operazioni sul monitor, ma alla chiamata della signal vengono attivati il processo chiamante che continua la sua operazione, sia il primo processo nella queue, perciò esistono due implementazioni possibili per risolvere il problema:
![[Signal wait-continue.excalidraw]]
Dato che il processo prima di poter essere eseguito deve passare per tutta la *entry queue*, altri processi potrebbero aver modificato la condition necessaria per l'ingresso nello stato di esecuzione, perciò è necessario che la condizione venga verificata anche prima dell'esecuzione
``` java
while (!condition)
	await()
// Accesso alla risorsa
```

![[Monitor esempio.png]]