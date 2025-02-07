In Linux il file system è detto omogeneo, cioè tutto quello che si vede è rappresentato da un file
* File
* Cartelle
* Dispositivi

Ogni file è associato ad almeno un nome, ma può averne anche di più attraverso i symlinks, inoltre ogni file possiede
* Un descriptor (i-node)
* Un id (i-number)

Ogni i-node contiene:
* Tipo di file (fra quelli sopra indicati).
* Proprietario e gruppo (con appositi id).
* Dimensione del file.
* Data di ultima modifica.
* 12 bit di protezione.
* Numero di symlinks.
* 13/15 indirizzi a blocchi, dove i primi 10 indirizzi indicano 10 blocchi e i rimanenti indicano 128 blocchi ciascuno (3/5 livelli di indirettezza).

La tecnica di allocazione è quella ad [[File System|indice]], i blocchi fisici variano da 0.5 a 4kb, ed esistono 4 regioni
* Boot block: contiene il programma di inizializzazione del sistema.
* Super block: contiene i limiti delle regioni, un puntatore alla lista di blocchi liberi e un puntatore alla lista di i-node liberi.
* I-list lista di tutti gli i-nodes.
* Data blocks: area dove sono memorizzati i file.

Allora se un file system è composto da blocchi di 0.5kb e ha 3 livelli di indirettezza, la dimensione massima di un file sarà
$$
10*0.5+128*0.5+128^2*0.5+128^3*0.5=1GB+8MB+64KB+5KB
$$
---
## Protezione dei file
Ogni file può essere acceduto in tre modalità:
* lettura
* scrittura
* esecuzione

Il proprietario e il superuser possono modificare l'accesso di ciascun tipo agli altri utenti, questi permessi sono indicati nei 12 bit di protezione:
* La prima terna indica il *suid*, *sgid*, *sticky*, se suid è settato, al momento di esecuzione il file avrà l'user id del proprietario, se sgid è settato all' esecuzione il processo avrà il group id del proprietario, se invece sticky è settato il processo sarà mantenuto nella memoria di swap anche dopo la terminazione.
* Le altre 3 terna indicano i permessi di *r* read, *w* write, *x* execute per il proprietario, gruppo e tutti gli altri.
---
## Accesso al file system
Per gestire l'accesso ai file il sistema operativo fa utilizzo di 3 strutture dati:
* Tabella dei file aperti per processo: contiene un record per ogni file utilizzato dal processo.
* Tabella dei file aperti nel sistema: contiene un record per ogni sessione di utilizzo di un file nel sistema.
* Tabella dei file attivi: contiene un record per ogni file aperto nel sistema.

L'apertura di un file provoca quindi
1. L'aggiunta del i-node nella tabella dei file attivi, solo se non è già presente.
2. L'aggiunta nella tabella dei file di sistema della sessione, che contiene un *I/O pointer* e l'indirizzo dell'i-node nella tabella dei file attivi.
3. L'aggiunta del file descriptor nella tabella dei file del processo, con indirizzo alla tabella dei file di sistema.