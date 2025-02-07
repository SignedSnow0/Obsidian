In Linux lo scambio di messaggi è disponibile attraverso due metodi differenti: i segnali e i pipe.

---
## Segnali
Un processo che desidera ricevere un segnale si iscrive ad esso chiamando la funzione *signal* e indicando un PFN che eseguirà del comportamento custom in risposta.
![[Signal.png]]
Esistono diversi tipi di segnali al quale uno si può iscrivere, per esempio:
* *SIGUSR1* e *SIGUSR2* sono segnali senza comportamento di default, creati per scambio di messaggi fra programmatori.
* *SIGKILL* e *SIGSTOP* sono mandati dal sistema operativo quando si desidera terminare il processo, questi segnali non sono né ignorabili né customizzabili.
* *SIGCHLD* è inviato al processo padre quando un suo figli termina l'esecuzione.

Un processo per inviare segnali utilizza la syscall *kill*
``` c
int kill(int pid, int signum)
```
* se *pid*>0 il segnale verrà inviato solo al processo indicato.
* se *pid*==0 il segnale verrà inviato ai processi del gruppo del mittente.
* se *pid*<-1 il segnale verrà inviato ai processi del gruppo pari al valore assoluto del *pid*
* *pid*=-1 è undefined behaviour.

Esistono infine altre funzioni utili:
``` c
unsigned int alarm(unsigned int seconds)
```
Imposta una sveglia che si attiverà dopo *seconds* secondi, allora il processo riceverà un segnale di tipo *SIGALARM*.
``` c
int pause()
```
Sospende il processo fino alla ricezione di un segnale.

---
## Pipe