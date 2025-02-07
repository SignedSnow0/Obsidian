In Java il [[Modello a memoria comune|semaforo]] è implementato come una classe astratta che fornisce due metodi:
``` java
void acquire(int permits = 1);
```
``` java
void release(int permits = 1);
```
che aggiungono e sottraggono valori al semaforo, inoltre il costruttore accetta un numero iniziale di permessi.
Sotto è presentato un esempio di semaphore che riproduce il comportamento di un mutex o un metodo *synchronized*, questo pattern è chiamato semaforo privato.
![[Semaphore.png]]