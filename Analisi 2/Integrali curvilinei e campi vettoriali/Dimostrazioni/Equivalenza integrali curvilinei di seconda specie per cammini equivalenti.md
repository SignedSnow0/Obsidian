---
subject: analisi 2
type: dimostrazione
---
Sia $\alpha:[a,b]\to\mathbb{R}^n,\beta:[c,d]\to\mathbb{R}^n$ [[Cammini equivalenti|cammini equivalenti]] a tratti, sia $f:\alpha([a,b])\to\mathbb{R}^n$, allora
$$
\int f\cdot d\beta=\begin{cases}\displaystyle\int f\cdot d\alpha\quad u\text{ è crescente}\\\displaystyle-\int f\cdot d\alpha\quad u \text{ è decrescente}\end{cases}
$$
# Dimostrazione
Sia $u$ la funzione usata nella definizione di [[Cammini equivalenti|cammini equivalenti]], notiamo che $u_{|(c,d)}$ è un cambiamento di variabile, inoltre
$$
\forall s\in[c,d]\quad\beta'(s)=u'(s)\alpha'(u(s))
$$
quindi
$$
\int f\cdot d\alpha=\int_{[a,b]}f(\alpha(t))\cdot\alpha'(t)dt=\int_{(a,b)}f(\alpha(t))\cdot\alpha'(t)dt
$$
$$
=\int_{(c,d)}f(\alpha(u(s)))\cdot\alpha'(u(s))|u'(s)|ds
$$
dunque se $u$ è crescente
$$
=\int_{(c,d)}f(\alpha(u(s)))\cdot\alpha'(u(s))u'(s)ds=\int_{(c,d)}f(\beta(s))\cdot\beta'(s)ds=\int f\cdot d\beta
$$
mente se $u$ è decrescente
$$
=-\int_{(c,d)}f(\alpha(u(s)))\cdot\alpha'(u(s))u'(s)ds=-\int_{(c,d)}f(\beta(s))\cdot\beta'(s)ds=-\int f\cdot d\beta\quad\square
$$

##### Correlati: