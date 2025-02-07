---
subject: analisi 1
type: dimostrazione
---
Sia $b_n>0,b_n\to\infty,b_n$ strettamente crescente, se $\displaystyle\exists\lim_{n\to\infty}\frac{a_{n+1}-a_n}{b_{n+1}-b_n}=l\in\overline{\mathbb{R}}$, allora $\displaystyle\exists\lim_{n\to\infty}\frac{a_n}{b_n}=l$
# Dimostrazione
Per definizione di limite:
$$
\forall\epsilon>0\quad\exists n_\epsilon:\left|\frac{a_{n+1}-a_n}{b_{n+1}-b_n}-l\right|<\epsilon\quad\forall n\ge n_\epsilon
$$
Allora, dato che $b_n$ è a termini positivi:
$$
(l-\epsilon)(b_{n+1}-b_n)<a_{n+1}-a_n<(l+\epsilon)(b_{n+1}-b_n)
$$
$$
(l-\epsilon)\sum_{n=n_\epsilon}^{k-1}(b_{n+1}-b_n)<\sum_{n=n_\epsilon}^{k-1}(a_{n+1}-a_n)<(l+\epsilon)\sum_{n=n_\epsilon}^{k-1}(b_{n+1}-b_n)
$$
Dato che la serie è telescopica:
$$
(l-\epsilon)(b_k-b_{n_\epsilon})<a_k-a_{n_\epsilon}<(l+\epsilon)(b_k-b_{n_\epsilon})
$$
$$
(l-\epsilon)(1-\frac{b_{n_\epsilon}}{b_k})<\frac{a_k}{b_k}-\frac{a_{n_\epsilon}}{b_k}<(l+\epsilon)(1-\frac{b_{n_\epsilon}}{b_k})
$$
$$
(l-\epsilon)(1-\frac{b_{n_\epsilon}}{b_k})+\frac{a_{n_\epsilon}}{b_k}<\frac{a_k}{b_k}<(l+\epsilon)(1-\frac{b_{n_\epsilon}}{b_k})+\frac{a_{n_\epsilon}}{b_k}
$$
Perciò
$$
l-\epsilon<\frac{a_k}{b_k}<l+\epsilon\quad\square
$$