---
subject: analisi 2
type: dimostrazione
---
Sia $\alpha:[a,b]\to\mathbb{R}^n,\beta:[c,d]\to\mathbb{R}^n$ [[Cammini equivalenti|cammini equivalenti]] continui a tratti, $f:\alpha([a,b])=\beta([c,d])\to\mathbb{R}$, allora
$$
\int_{\alpha}f(x)ds=\int_{\beta}f(x)ds
$$
# Dimostrazione
Sia $u$ la funzione usata nella definizione di [[Cammini equivalenti|cammini equivalenti]], notiamo che $u_{|(c,d)}$ è un cambiamento di variabile, inoltre
$$
\forall s\in[c,d]\quad\beta'(s)=u'(s)\alpha'(u(s))
$$
quindi
$$
||\beta'(s)||=||\alpha'(u(s))|||u'(s)|
$$
per il [[Teorema del cambiamento di variabile|teorema del cambiamento di variabile]]
$$
\int_{\alpha}f(x)ds=\int_{[a,b]}f(\alpha(t))||\alpha'(t)||dt=\int_{(a,b)}f(\alpha(t))||\alpha'(t)||dt
$$
$$
=\int_{(c,d)}f(\alpha(u(s)))||\alpha'(u(s))|||u'(s)|ds=\int_{[c,d]}f(\beta(s))||\beta'(s)||ds=\int_{\beta}f(x)ds\quad\square
$$

##### Correlati: