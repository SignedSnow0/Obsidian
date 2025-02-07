---
subject: analisi 2
type: definizione
---
Sia $A\subseteq\mathbb{R}^n,v\in\mathbb{R}^n,x_0\in A$, poniamo la retta passante per $x_0$ in $A$
$$
A_{x_0,v}=\{t\in\mathbb{R}|x_0+tv\in A\}
$$
Sia allora $f:A\to\mathbb{R}$ e poniamo per $t\in A_{x_0,v}\setminus\{0\}$
$$
r_{x_0,v}(t)=\frac{f(x_0+tv)-f(x_0)}{t}
$$
e supponiamo che $0\in D(A_{x_0,v})$, allora se esiste
$$
\lim_{t\to0}r_{x_0,v}(t)
$$
lo chiameremo derivata di $f$ rispetto a $v$ in $x_0$ e lo indicheremo con $\frac{df}{dv}(x_0)$