---
subject: analisi 1
type: dimostrazione
---
Sia $x_0\in\mathring{D}, f$ derivabile in $x_0$, se $x_0$ è punto di estremo, allora $f'(x_0)=0$
# Dimostrazione
Sia $x_0$ punto di massimo, allora per qualche $r>0$
$$
\frac{f(x)-f(x_0)}{x-x_0}\ge0\quad\forall x\in(x_0-r,x_0)
$$
$$
\frac{f(x)-f(x_0)}{x-x_0}\le0\quad\forall x\in(x_0,x_0+r)
$$
cioè 
$$
\lim_{x\to x_0^-}\frac{f(x)-f(x_0)}{x-x_0}\ge0,\quad\lim_{x\to x_0^+}\frac{f(x)-f(x_0)}{x-x_0}\le0
$$
ma visto che la funzione è continua abbiamo che
$$
0\le\lim_{x\to x_0^-}\frac{f(x)-f(x_0)}{x-x_0}=f'(x_0)=\lim_{x\to x_0^+}\frac{f(x)-f(x_0)}{x-x_0}\le0
$$
quindi per il [[Teorema dei Carabinieri]] $f'(x_0)=0\quad\square$