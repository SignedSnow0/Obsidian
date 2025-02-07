---
subject: analisi 2
type: dimostrazione
---
Sia $A\subseteq\mathbb{R}^n$, allora $\text{Fr}(A),\overline{A}$ sono sottoinsiemi chiusi di $A$.
# Dimostrazione
* Proviamo che $\text{Fr}(A)$ sia chiuso
Sia $x^0\in\text{Fr}(\text{Fr}(A)),r\in\mathbb{R}^+$, allora
$$
\exists x^1\in\text{Fr}(A)\cap B(x^0,r)
$$
visto che $B(x^0,r)$ è aperto
$$
\exists r_0\ge0:B(x^1,r_0)\subseteq B(x^0,r)
$$
essendo $x^1\in\text{Fr}(A)$ allora $B(x^1,r_0)$ contiene sia elementi interni che esterni ad $A$ che appartengono anche a $B(x^0,r)$, dunque
$$
\forall r>0\quad B(x^0,r)\cap A\ne\emptyset,\quad B(x^0,r)\cap\mathbb{R}^n\setminus A\ne\emptyset\implies x^0\in\text{Fr}(A)
$$
* Proviamo che $\overline{A}$ sia chiuso
Sia $x^0\in\text{Fr}(\overline{A})$, allora o $x^0\in A$, e quindi $x^0\in\overline{A}$, oppure $x^0\notin A$.
Sia $r>0$, allora $B(x^0,r)$ contiene un punto non in $A$: $x_0$, poichè $x^0\in\text{Fr}(\overline{A})$
$$
\exists x^1\in\overline{A}\cap B(x^0,r)
$$
allora se $x^1\in A$ abbiamo trovato elementi di $B(x^0,r)$ sia in a che non, altrimenti definiamo $\rho\in\mathbb{R}^+:B(x^1,\rho)\subseteq B(x^0,r)$, poichè $x^1\in\text{Fr}(A)\quad B(x^1,\rho)$
$$
\exists x^2\in A\cap B(x^0,r)
$$
perciò in ogni caso $B(x^0,r)$ contiene sia elementi di $A$ che non, perciò $x^0\in\overline{A}\quad\square$

##### Correlati:
* [[Frontiera]]
* [[Chiusura]]