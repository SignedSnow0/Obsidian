---
subject: analisi 2
type: dimostrazione
---
Sia $A\subseteq\mathbb{R}^n$, allora
$$
A\space\text{è aperto}\iff A\cap\text{Fr}(A)\ne\emptyset
$$
# Dimostrazione
* Sia $A$ aperto e $x\in A$,allora $x\in\mathring{A}$, perciò
$$
\exists r>0:B(x,r)\subseteq A\implies x\notin\text{Fr}(A)
$$
perciò $A\cap\text{Fr}(A)=\emptyset$.
* Sia ora $A\cap\text{Fr}(A)=\emptyset,x\in A$, allora $B(x,r)\subseteq A$ oppure $B(x,r)\subseteq\mathbb{R}^n\setminus A$, ma la seconda condizione non si può verificare perchè $x\in A$, ne segue allora che
$$
x\in\mathring{A}\quad\square
$$

##### Correlati:
* [[Frontiera]]
* [[Analisi 2/Funzioni di più variabili reali/Insieme aperto]]