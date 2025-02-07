I modelli a memoria comune sono [[Processi|processi leggeri]], iniziamo con delle definizioni di componenti di un programma multithreaded.
> [!definition] Processo
> Un processo è la parte attiva del programma che esegue operazioni spesso usufruendo di risorse.

> [!definition] Risorsa
> Le risorse sono dati del programma o oggetti forniti dal sistema operativo utilizzate dai processi per svolgere il loro lavoro, sono divise in:
> * Private: utilizzate da un singolo processo.
> * Comuni: utilizzate da più processi.

Per garantire il corretto funzionamento del programma le risorse comuni devono essere utilizzate solamente da un singolo processo alla volta, perciò è necessario una struttura dati che garantisca la mutua esclusione, chiamata **mutex**.

---
## Strutture di sincronizzazione
> [!definition] Mutex
> Un mutex è una struttura che garantisce l'utilizzo di una risorsa in maniera esclusiva trattando il codice al suo interno (sezione critica) come un'operazione atomica (indivisibile) che una volta iniziata blocca l'esecuzione della stessa sezione per ogni altro processo.

Questa implementazione del mutex è chiamata hardware-based perché necessita che la cpu non interrompa il programma durante la sezione critica, ed è la soluzione più usata.
Esistono inoltre soluzioni puramente algoritmiche (algoritmo di Dekker) e soluzioni che sfruttano risorse del sistema operativo (semafori).

> [!definition] Semaforo
> Un semaforo è uno strumento di sincronizzazione fornito dal sistema operativo, al suo nocciolo è formato da due operazioni atomiche
> * Un'operazione di accesso che sospende il processo chiamante finché il valore interno del semaforo diventi positivo (e poi decrementi il valore).
> * Un'operazione di segnalazione che incrementa il valore interno di 1.

Il semaforo è l'unità più semplice in grado di risolvere qualsiasi problema di concorrenza, infatti un mutex può essere visto come un caso particolare di semaforo che assume solo i valori 0 e 1.