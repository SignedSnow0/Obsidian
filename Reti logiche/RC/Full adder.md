---
subject: reti logiche
type: definizione
---
Il full adder è una [[Rete combinatoria]] che permette di eseguire la somma di un bit.
Un full adder completo ha diversi ingressi e uscite:
* $C_\text{in}$, flag di riporto in ingresso, utile per concatenare diversi adder.
* $A$, primo valore da sommare.
* $B$, secondo valore da sommare.
* $C_\text{out}$, flag di riporto in uscita.
* $\text{Out}$ valore in uscita.

Come possiamo notare l'implementazione di un Full adder è quella di un [[Half Adder]] con i bit di riporto in modo da rendere possibile la concatenazione per realizzare adder a $n$ bit.