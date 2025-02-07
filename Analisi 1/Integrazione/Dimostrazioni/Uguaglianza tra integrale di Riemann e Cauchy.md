---
subject: analisi 1
type: dimostrazione
---
Ogni integrale di Cauchy è integrabile secondo Riemann e hanno lo stesso valore
$$
\mathcal{C}([a,b])\subseteq\mathcal{R}([a,b]),\quad\int_a^bf(x)dx=\int_{[a,b]}f(x)dx
$$
# Dimostrazione
Notiamo che le approssimazioni di Cauchy sono funzioni a scala della forma
$$
x_k=a+\frac{b-a}{n}k
$$
Inoltre $\forall h\in S_f^+\quad h\ge S_n,\quad\forall g\in S_f^-\quad g\le s_n$, scegliendo però $\inf$ e $\sup$ abbiamo che
$$
\underline{\int_{[a,b]}}f(x)dx=s_n,\quad\overline{\int_{[a,b]}}f(x)dx=S_n
$$
Perciò abbiamo che
$$
s_n\le\underline{\int_{[a,b]}}f(x)dx\le\overline{\int_{[a,b]}}f(x)dx\le S_n\quad\square
$$