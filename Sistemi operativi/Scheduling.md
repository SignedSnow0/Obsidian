> [!definition] Scheduler
> Lo scheduler è un programma del SO che si occupa di gestire il tempo di esecuzione della CPU fra i [[Processi|processi]] pronti per l'esecuzione, lo scheduling è diviso in 3 fasi:
> 1. Scheduling a brave termine (di CPU).
> 2. Scheduling a medio termine (swapping).
> 3. Scheduling a lungo termine [opzionale].

> [!definition] Scheduler a breve termine
> Questa parte dello scheduler si occupa della scelta del prossimo processo [[Processi|in stato di ready]] che verrà eseguito dalla CPU e del suo cambio di contesto.
> Inoltre sposta i processi dallo stato di [[Processi|waiting]] allo stato di [[Processi|ready]] qualora la risorsa attesa sia diventata disponibile.
> Inoltre lo scheduler a breve termine per garantire un utilizzo condiviso delle risorse può spostare processi in esecuzione allo stato di ready forzatamente in un meccanismo chiamato **preemption**.
 
> [!definition] Scheduler a medio termine
> Lo scheduler a medio termine si occupa di spostare i processi non in uso nella memoria secondaria permettendo il caricamento di nuovi processi qualora la memoria primaria non fosse sufficiente.