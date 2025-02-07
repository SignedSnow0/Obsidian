Linux, come tutti i sistemi operativi moderni, permette la creazione di più [[Processi|processi]] e più [[Processi|thread]] per ogni processo.

---
In C la creazione di un processo è permessa attraverso la syscall *fork*, il valore restituito è un intero:
* Se il valore è nullo, allora significa che è in esecuzione il processo figlio.
* Se invece il numero è positivo, indica il [[Processi|pid]] del figlio creato.

![[Fork.png]]

Il processo padre può attendere la fine del processo figlio attraverso la system call *wait*
![[Wait.png]]
Il processo figlio termina la propria esecuzione tramite la system call *exit* che prevede come parametro un intero che indica il suo stato.
Le macro *WIFEXITED* e  *WEXITSTATUS* permettono di vedere se il processo figli è terminato correttamente e con che stato finale.

Ovviamente è possibile che un padre abbia più figli in parallelo:
![[Wait multiplo.png]]
