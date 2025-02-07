---
subject: analisi 2
type: dimostrazione
---
Sia $A\subseteq\mathbb{R}^n$ aperto [[Insieme connesso per archi|connesso per archi]], $F\in\mathcal{C}(A)$ [[Campo vettoriale|campo vettoriale]], allora sono equivalenti
1. $F$ è [[Campo vettoriale esatto|esatto]]
2. $F$ è [[Campo vettoriale conservativo|conservativo]]
# Dimostrazione
Sia $F$ esatto, $\alpha\in\mathcal{C}^1$, allora per la [[Analisi 2/Calcolo differenziale/Dimostrazioni/Chain rule|chain rule]]
$$
(U\circ\alpha)'(t)=\nabla U(\alpha(t))\cdot\alpha'(t)=F(\alpha(t))\cdot\alpha'(t)
$$
perciò
$$
\int F\cdot d\alpha=\int_a^bF(\alpha(t))\cdot\alpha'(t)dt=\int_a^b(U\circ\alpha)'(t)dt=U(\alpha(b))-U(\alpha(b))
$$
inoltre vale anche per cammini continui a tratti
$$
\int F\cdot d\alpha=\sum_{j=1}^{k}\int F\cdot d\alpha^j=\sum_{j=1}^{k}[U(\alpha(t_j))-U(\alpha(t_{j-1}))]=U(\alpha(t_k))-U(\alpha(t_0))=U(\alpha(b))-U(\alpha(a))
$$
dimostrando che $F$ è conservativo.
Sia ora $F$ conservativo, $x^0\in A$ prendiamo per $x$ un cammino $a^x\in\mathcal{C}^1$ a tratti con sostegno in $A$ con estremi $x^0,x$, sia
$$
U:A\to\mathbb{R},\quad U(x)=\int F\cdot d\alpha^x
$$
sia $i\in\{1,\dots,n\},x\in A,\delta\in\mathbb{R}^+:B(x,\delta)\subseteq A$, se $t\in\mathbb{R},|t|<\delta$ allora $[x,x+te^i]\subseteq A$, poniamo allora
$$
\alpha^{x+te^i}:[a,b+1]\to\mathbb{R}^n,\quad\alpha^{x+te^i}=\begin{cases}\alpha^x(s)\quad s\in[a,b]\\ x+(s-b)te^i\quad s\in[b,b+1]\end{cases}
$$
allora $\alpha^{x+te^i}$ è un cammino continuo a tratti di estremi $x^0,x+te^i$ e con sostegno in $A$, si ha allora
$$
U(x+te^i)-U(x)=\int F\cdot d\alpha^{x+te^i}-\int F\cdot d\alpha^{x}
$$
$$
=\int_{[b,b+1]}F(x+(s-b)te^i)\cdot(te^i)ds=t\int_b^{b+1}F_i(x+(s-b)te^i)ds 
$$
segue 
$$
\frac{U(x+te^i)-U(x)}{t}=\int_b^{b+1}F_i(x+(s-b)te^i)ds=\frac 1t\int_0^tF_i(x+\sigma e^i)d\sigma
$$
poichè $\sigma\to F_i(x+\sigma e^i)$ è continua in $(-\delta,\delta)$ per il [[Teorema fondamentale del calcolo integrale|teorema fondamentale del calcolo integrale]] si ha 
$$
\lim_{t\to0}\frac{U(x+te^i)-U(x)}{t}=\lim_{t\to0}\frac 1t\int_0^tF_i(x+\sigma e^i)d\sigma=F_i(x)
$$
che equivale a 
$$
\frac{\partial U}{\partial x_i}(x)=F_i(x)\quad\square
$$

##### Correlati: