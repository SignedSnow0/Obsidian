---
subject: matematica applicata
type: definizione
---
Data una [[Variabile casuale|v.c.]] $X$ si definisce, se esiste, il valore atteso come
$$
\E[X]=\begin{cases}\displaystyle\sum_{k=1}^nx_kp(x_k)\\\displaystyle\int_\mathbb{R}xf(x)dx\end{cases}
$$
### Proprietà
1. $$
\E[g(X)]=\begin{cases}\displaystyle\sum_{k=1}^ng(x_k)p(x_k)\\\displaystyle\int_\mathbb{R}g(x)f(x)dx\end{cases}
$$
2. $$
\forall\alpha,\beta\in\mathbb{R}\quad\E[\alpha X+\beta]=\alpha\E[X]+\beta
$$
3. $$
\E[h(X,Y)]=\begin{cases}\displaystyle\sum_{j=1}^n\sum_{k=1}^nh(x_k,y_j)p(x_k,y_j)\\\displaystyle\iint_{\mathbb{R}^2}h(x,y)f(x,y)dxdy\end{cases}
$$
4. $$
\E[X+Y]=\E[X]+\E[Y]
$$