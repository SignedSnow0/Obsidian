---
subject: analisi 1
type: dimostrazione
---
Sia $f\in\mathcal{C}([a,b])$, se $f(a)f(b)<0$, allora esiste $c\in[a,b]:f(c)=0$.
# Dimostrazione
Sia $f(a)<0<f(b)$, definiamo
$$
a_0=a,b_0=b,c_0=\frac{a_0+b_0}2
$$
A questo punto:
* Se $f(c)=0$ abbiamo finito
* Se $f(c)<0$ sia $a_1=c_0,\quad b_1=b_0$
* Se $f(c)>0$ sia $a_1=a_0,\quad b_1=c_0$
Iterando il procedimento abbiamo che
$$
[a_n,b_n]\subseteq\dots\subseteq[a,b],\quad f(a_n)<0<f(b_n),\quad b_n-a_n=\frac{b-a}{2^n}
$$
Inoltre sappiamo che
$$
\lim_{n\to\infty}(b_n-a_n)=0, \quad 0\le\lim_{n\to\infty}b_n=0\le f(x_0)\le\lim_{n\to\infty}a_n\le0
$$
per qualche $x_0\in[a_n,b_n]$, allora per il [[Teorema dei Carabinieri]] $f(x_0)=0\quad\square$