---
subject: matematica applicata
type: definizione
---
La funzione densità è una funzione $f:\mathbb{R}\to\mathbb{R}^+_0$ tale che
$$
\forall A\subseteq\mathbb{R}\quad P(X\in A)=\int_Af(x)dx
$$
Per più [[Variabile casuale|variabili]] la funzione è $f:\mathbb{R}^n\to\mathbb{R}^+_0$ tale che
$$
\forall C\subseteq\mathbb{R}^n\quad P((X_1,\dots,X_n)\in C)=\int_Cf(x_1,\dots,x_n)dx_1\dots dx_n
$$
### Proprietà
1. $\displaystyle P(X=x)=\int_x^xf(x)dx=0$
2. $f(x)\ge0$
3. $\displaystyle P(X\in\mathbb{R})=\int_\mathbb{R}f(x)dx=1$
4. $\displaystyle P(X\le x)=\int_{-\infty}^xf(s)ds=F(x)$ quindi la [[Funzione di distribuzione|funzione di distribuzione]] è la [[Primitiva|primitiva]] della funzione densità.

Sapendo che la densità è la derivata della [[Funzione di distribuzione|distribuzione]] possiamo ridurre la dimensione del problema utilizzando il [[Teorema di Tonelli|teorema di Tonelli]]
$$
f_{x_j}(x_k)=\frac{dF_{x_j}}{dx_k}(x_k)=\frac{d}{dx_k}F(+\infty,x_k)=
$$
$$
=\frac{d}{dx_k}\int_{-\infty}^{x_k}\int_{-\infty}^{+\infty}f(x_j,s_k)dx_jds_k=\int_{-\infty}^{+\infty}f(\cdot,x_j)dx_j
$$