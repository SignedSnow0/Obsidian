> [!definition] Processo
> In un sistema operativo il processo è l'istanza di esecuzione di un programma, è composto da:
> * Codice del programma
> * Dati del programma (variabili globali e costanti)
> * Program counter
> * Valore dei registri
> * Stato dello stack
> * Risorse associate (file, connessioni di rete)
> 
> Le informazioni di esecuzione del processo sopra elencate assieme ad un'identificativo (**PID**) sono raggruppate nel **descrittore**.

> [!definition] Thread
> Un thread è un processo detto leggero che **condivide** con thread dello stesso tipo **codice**, **dati** e **risorse**.

Un processo durante la sua vita farà parte di vari stati:
1. Init: stato di caricamento del processo in memoria e inizializzazione dei dati.
2. Ready: il processo è inizializzato ed è pronto per essere eseguito.
3. Running: il processo è in esecuzione nella CPU.
4. Waiting: il processo è sospeso in attesa di un evento o risorsa.
5. Terminated: il processo è finito ma è ancora presente in memoria.

![[Stati processo.excalidraw]]

> [!definition] Bounds dei processi
> I processi possono essere caratterizzati dal tipo di risorsa che utilizzano maggiormente e quindi dalla quale sono dipendenti:
> * I processi **I/O bound** sono processi che impiegano la maggior parte del tempo del tempo in operazioni di I/O, perciò saranno molto nello stato di **waiting**.
> * I processi **CPU bound** invece impiegano la maggior parte del tempo utilizzando la **CPU**, perciò verranno spostati nello stato di **ready** da meccanismi di [[Scheduling|preemption]].