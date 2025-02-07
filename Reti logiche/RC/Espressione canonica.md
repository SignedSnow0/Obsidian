---
subject: reti logiche
type: definizione
---
Esistono due forme di espressioni canoniche: somma di prodotti e prodotto di somme.

### $1^a$ forma canonica (SP)
Ogni funzione di $n$ variabili è scrivibile come somma di tanti prodotti quante sono le configurazioni per cui la funzione valga 1, ogni prodotto è un [[Mintermine]] e appare ogni variabile in forma vera se vale 1 o negata se vale 0.

Inoltre un espressione canonica SP è la somma di [[Implicante primo essenziale]]

Grazie al [[Teorema di espansione di Shannon]] possiamo scrivere ogni funzione SP come
$$
F(x_1,\dots,x_n)=\sum_{i=0}^{2^n-1}m(i)\cdot F(i)
$$
dove $m(i)$ è l'i-esimo [[Mintermine]] di $n$ bit e $F(i)$ è il valore della funzione con input per cui il [[Mintermine]] vale 1.

### $2^a$ forma canonica (PS)
Ogni funzione di $n$ variabili è scrivibile come prodotto di tante somme quante sono le configurazioni per cui la funzione valga 0, ogni somma è un [[Maxtermine]] e appare ogni variabile in forma vera se vale 0 o negata se vale 1.

Inoltre un espressione canonica PS è la somma di [[Implicato primo essenziale]]

Ogni funzione in forma canonica avrà sempre un numero di [[Gate logici]] in cascata $\le2$.

Grazie al [[Teorema di espansione di Shannon]] possiamo scrivere ogni funzione PS come
$$
F(x_1,\dots,x_n)=\prod_{i=0}^{2^n-1}(M(i)+F(i))
$$
dove $M(i)$ è l'i-esimo [[Maxtermine]] di $n$ bit e $F(i)$ è il valore della funzione con input per cui il [[Maxtermine]] vale 0.