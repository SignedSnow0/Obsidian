>[!definition] Sistema operativo
>Un sistema operativo è un programma che agisce come intermediario fra l'user e l'hardware.
> * Permette l'accesso e la gestione di componenti fisici del computer.
> * Permette l'esecuzione di programmi degli utenti.

I sistemi operativi moderni si dicono *multiprogrammati*, cioè permettono l'esecuzione di più programmi contemporaneamente cambiando periodicamente il processo in esecuzione dalla cpu, per fare ciò effettuano il context swtiching
>[!definition] Context switch
> Il cambio di contesto è un'operazione effettuata da sistema operativo per garantire la multiprogrammazione, durante uno switch i registri della cpu vengono salvati in memoria e viene caricato un altro programma al suo posto.
> Questa operazione può essere eseguita per due motivi:
> * Il processo deve attendere una risorsa non disponibile al momento.
> * Il processo viene forzatamente sospeso per fare spazio ad altri processi (preemption).

Inoltre per garantire un sistema multiprogrammato funzionale sono necessari:
1. Gestione e protezione della memoria, che è condivisa fra i diversi processi.
2. [[Scheduling|Scheduling]] della cpu.
3. [[Messaggi|Interazione]] fra processi.
4. Possibilità di accedere alle [[File System|Risorse]] gestite dal sistema operativo.

I programmi possono chiedere al sistema operativo di eseguire delle operazioni tramite le *system call*.
>[!definition] System call
> 1. Il processo indica quale system call vuole chiamare.
> 2. Il processo manda un'interrupt per effettuare la chiamata.
> 3. Alla ricezione dell'interrupt il sistema operativo effettua in context switch.
> 4. Viene eseguita una routine che individua la parte del sistema operativo da eseguire.
> 5. Il programma chiamante viene ripristinato.

Questo processo è necessario perchè i sistemi operativi implementano *meccanismi di protezione* rispetto ai programmi ed operazioni degli utenti, perciò spesso le routines effettuate dalle system calls sono "speciali" e possono essere eseguite solo dal sistema operativo.
> [!definition] Modalità di esecuzione
> Le cpu moderne prevedono un registro di flag che indica i permessi di esecuzione 
> 1. User mode: 1 
> 2. Kernel mode: 0
> 
> Alcune esecuzioni permesse solo in kernel mode sono:
> * Accesso a periferiche.
> * Gestione della memoria
> * Disabilitazione di interrupts.
---
## Strutture del sistema operativo
Dal punto di vista strutturale esistono 4 tipi di sistemi operativi:
* Struttura monolitica.
* Struttura modulare.
* Microkernel.
* Macchina virtuale.

Nella struttura monolitica il sistema operativo è un unico programma che contiene tutti i requisiti prima specificati, i sistemi linux based sono monolitici.
Nella struttura modulare il sistema operativo è diviso in moduli, ognuno che svolge un requisito del sistema operativo, di solito il modello è a strati.
La struttura a microkernel cerca di limitare al minimo le operazioni eseguite in modalità kernel, permettendo quindi che certe componenti del sistema operativo si comportino come semplici programmi, implementazioni simili sono quelle scelte da windows e macos.
Le macchine virtuali sono un insieme di hardware virtualizzato e sistema operativo che girano come un programma all'interno di un altro sistema operativo, per migliorare le prestazioni, l'hardware moderno contiene sistemi di virtualizzazione appositi per l'utilizzo di vms.