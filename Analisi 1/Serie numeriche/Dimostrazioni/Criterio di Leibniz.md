---
subject: analisi 1
type: dimostrazione
---
Sia $\displaystyle\sum_{k=0}^{\infty}(-1)^kb_k$ una serie a segni alterni, assumiamo che
* $\displaystyle\lim_{k\to\infty}b_k=0$
* $b_k$ sia monotona decrescente
Allora la serie converge.
# Dimostrazione
Dato che la serie è monotona decrescente abbiamo che
$$
s_{2n}\le s_{2n-2}
$$
$$
s_{2n+1}\ge s_{2n-1}
$$
Perciò le due serie $\{s_{2n}\},\{s_{2n+1}\}$ sono monotone decrescente e crescente, inoltre $\{s_{2n}\}$ è limitata inferiormente e $\{s_{2n+1}\}$ è limitata superiormente, perciò
$$
\lim_{n\to\infty}s_{2n}=\inf s_{2n}=s',\quad\lim_{n\to\infty}s_{2n+1}=\sup s_{2n+1}=s''
$$
Inoltre $s'=s''$
$$
s'-s''=\lim_{n\to\infty}s_{2n}-s_{2n+1}=\lim_{n\to\infty}b_{2n+1}=0
$$
Sia quindi $s=s'=s''$, allora la serie converge a $s\in\mathbb{R}\quad\square$