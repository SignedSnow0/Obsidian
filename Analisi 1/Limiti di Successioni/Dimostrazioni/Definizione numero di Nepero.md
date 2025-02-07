---
subject: analisi 1
type: dimostrazione
---
Sia la successione $a_n=\displaystyle(1+\frac1n)^n$, allora $a_n$ è monotona crescente e $2\le a_n<3$. Inoltre $\displaystyle\lim_{n\to\infty}{(1+\frac1n)^n}=e$
# Dimostrazione
Iniziamo dimostrando che la successione è monotona crescente
$$
\frac{a_n}{a_{n-1}}=\frac{(1+\frac1n)^n}{(1+\frac1{n-1})^{n-1}}=\frac{(\frac{n+1}n)^n}{(\frac{n-1+1}{n-1})^{n-1}}=\left(\frac{\frac{n+1}n}{\frac n{n-1}}\right)^n\frac1{(\frac n{n-1})^{-1}}=\left(\frac{n+1}n\frac{n-1}n\right)^n\frac1{\frac{n-1}n}=\left(\frac{n^2-1}{n^2}\right)^n\frac1{1-\frac1n}=\frac{(1-\frac1{n^2})^n}{1-\frac1n}\ge\frac{1-\frac{n}{n^2}}{1-\frac1n}=1
$$
Visto che $a_1=2$ e che la successione è monotona crescente abbiamo dimostrato che $a_n\ge2$.
Dimostriamo ora che $a_n<3$
$$
(1+\frac1n)^n=\sum_{k=0}^n\binom{n}{k}\frac1{n^k}=\sum_{k=0}^{n}\frac{n!}{k!(n-k)!n^k}<\sum_{k=0}^{n}\frac1{k!}=1+\sum_{k=1}^{n}\frac1{k!}\le1+\sum_{k=1}^n\frac1{2^{k-1}}=1+\sum_{k=0}^n\frac1{2^k}=1+2 \quad\forall n\ge1
$$