---
subject: analisi 1
type: dimostrazione
---
Sia $a,b\in\overline{\mathbb{R}},a<b,f(a,b)\to\mathbb{R}$ derivabile su $(a,b)$, allora
* $f$ è crescente su $(a,b)\iff f'(x)\ge0\quad\forall x\in(a,b)$
* Se $f'(x)>0\quad\forall x\in(a,b)$ allora $f$ è strettamente crescente.
# Dimostrazione
* Sia $f$ crescente, allora 
$$
\frac{f(x)-f(x_0)}{x-x_0}\ge0\quad\forall x\ne x_0
$$
perciò $f'(x_0)\ge 0$
* Sia $f'(x_0)\ge0\quad\forall x\in(a,b)$, allora per il [[Analisi 1/Derivazione/Dimostrazioni/Teorema di Lagrange]] $\forall x_1<x_2\in(a,b)$
$$
f(x_2)-f(x_1)=f'(\bar{x})(x_2-x_1)\ge0\quad\square
$$