---
subject: analisi 1
type: dimostrazione
---
Sia $a_n>0\quad\forall n\in\mathbb{N}$, supponiamo che $\displaystyle\exists\lim_{n\to\infty}\frac{a_{n+1}}{a_n}=l$, allora:
* Se $l<1\quad a_n\to0$
* Se $l>1\quad a_n\to\infty$
# Dimostrazione
* Sia $l<1$
Per definizione di limite:
$$
\forall\epsilon>0\quad\exists n_\epsilon:\left|\frac{a_{n+1}}{a_n}-l\right|<\epsilon\quad\forall n\ge n_\epsilon
$$
Dato che la successione è a termini positivi abbiamo che $a_{n+1}<(l+\epsilon)a_n$, con $(l+\epsilon)<1$, allora iterando sappiamo che
$$
a_{n+1}<(l+\epsilon)a_n<\dots<(l+\epsilon)^{k-1}a_{n-k}
$$
Perciò 
$$
a_n<(l+\epsilon)^{k-1}a_{n_k}\to0\quad\square
$$