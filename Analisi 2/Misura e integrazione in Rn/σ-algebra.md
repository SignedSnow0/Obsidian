---
subject: analisi 2
type: definizione
---
Sia $\Omega$ un insieme, si dice che una famiglia di sottoinsiemi $\mathcal{A}$ è una $\sigma$-algebra se
1. $\emptyset\in\mathcal{A}$
2. se $A\in\mathcal{A}$ allora anche $A^c=\Omega\setminus A\in\mathcal{A}$
3. se $a_k$ è una successione di elementi di $\mathcal{A}$ allora $\displaystyle\bigcup_{k\in\mathbb{N}}a_k\in\mathcal{A}$

Una misura su $\mathcal{A}$ è una funzione $\mu:\mathcal{A}\to[0,+\infty]:$
1. $\mu(\emptyset)=0$
2. se $a_k$ è una successione di elementi a due a due disgiunti si ha
$$
\mu(\bigcup_{k\in\mathbb{N}}a_k)=\sum_{k=1}^{\infty}\mu(a_k)
$$

##### Correlati:
* [[Teorema di Caratheodory]]