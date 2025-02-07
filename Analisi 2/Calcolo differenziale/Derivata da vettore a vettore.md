---
subject: analisi 2
type: definizione
---
Sia $A\subseteq\mathbb{R}^n,v\in\mathbb{R}^n,x^0\in A,f:A\to\mathbb{R}^m$, poniamo l'inisieme 
$$
A_{x^0,v}=\{t\in\mathbb{R}\space|\space x^0+tv\in A\}
$$
allora per $t\in A_{x_0,v}\setminus\{0\}$ creiamo la funzione
$$
r_{x_0,v}(t)=\frac{f(x^0+tv)-f(x^0)}{t}
$$
allora se $0\in D(A_{x^0,v})$ ed esiste il limite
$$
\lim_{t\to0}r_{x^0,v}(t)
$$
lo chiameremo derivata di $f$ rispetto al vettore $v$ in $x^0$, indicato con $\frac{\partial f}{\partial v}(x^0)$