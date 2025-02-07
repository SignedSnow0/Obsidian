---
subject: reti logiche
type: definizione
---
### Complemento a 1
Data una base $\beta$ per la rappresentazione di numero possiamo definirne in complemento a $\beta-1$ di un numero $A$ come $(\beta^n-1)-A$.

In particolare in base $\beta=2$ calcolare il complemento a 1 di un numero risulta particolarmente facile perchè basta farne il NOT bit a bit.
### Complemento a 2
Data una base $\beta$ di un numero $A$ il complemento a due è $\beta^n-A$, o anche il complemento a 1 più 1.

Perciò in base binaria il complemento a due risulta essere il NOT bit a bit del numero più 1.

Il complemento a due dei numeri è utile per rappresentare numeri con segno a porta a diversi vantaggi rispetto ad altre rappresentazioni come quella del segno e modulo.
* Per eseguire la sottrazione di due numeri basta eseguirne la somma tra il numero originale e il complemento a 2 del secondo, è quindi possibile usare un [[Full adder]] per eseguire anche sottrazioni.
* È possibile eseguire calcoli aritmetici con numeri positivi e negativi senza cambiare il comportamento delle reti.
* Non ci sono valori duplicati come per esempio lo zero nella rappresentazione di segno e modulo.

