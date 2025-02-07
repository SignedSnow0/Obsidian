---
subject: analisi 1
type: dimostrazione
---
Sia $f$ monotona su $[a,b]$, allora $f\in\mathcal{R}([a,b])$
# Dimostrazione
Sia $f$ crescente, allora poniamo $\forall\epsilon>0\quad\frac{b-a}{n}<\epsilon,\quad x_k=a+\frac{b-a}{n}k$, e
$$
h_n=\begin{cases}f(x_k)\quad x\in(x_{k-1},x_k]\\f(a)\quad x=a\end{cases}
$$
$$
g_n=\begin{cases}f(x_{k-1})\quad x\in[x_{k-1},x_k)\\f(b)\quad x=b\end{cases}
$$
Allora
$$
\int_a^bh_n(x)dx-\int_a^bg_n(x)dx=\sum_{k=1}^{n}f(x_k)\Delta x-\sum_{k=1}^{n}f(x_{k-1})\Delta x=\sum_{k=1}^n(f(x_k)-f(x_{k-1}))\Delta x=\frac{f(b)-f(a)}{n}(b-a)\le\epsilon(f(b)-f(a))
$$
Che soddisfa [[Integrale secondo Riemann]] $\square$