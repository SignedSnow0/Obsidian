---
subject: analisi 2
type: dimostrazione
---
Sia $A\subseteq\mathbb{R}^n$ aperto, $f\in\mathcal{C}^1(A),x,y,\in A:[x,y]\subseteq A$, allora esiste $z\in[x,y]$ tale che
$$
f(y)-f(x)=\nabla f(z)\cdot(y-z)
$$
# Dimostrazione
Sia $F:[0,1]\to\mathbb{R},F(t)=f(x+t(y-z))$, allora $F\in\mathcal{C}^1([0,1]),$
$$
F'(t)=\nabla f(x+t(y-x))\cdot(y-z)
$$
applicando il [[Analisi 1/Derivazione/Dimostrazioni/Teorema di Lagrange|teorema di Lagrange]] in $\mathbb{R}$
$$
\exists c\in[0,1]:f(y)-f(x)=F(1)-F(0)=\nabla f(x+c(y-x))\cdot(y-x)\quad\square
$$