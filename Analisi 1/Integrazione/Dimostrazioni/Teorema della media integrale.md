---
subject: analisi 1
type: dimostrazione
---
Sia $f\in\mathcal{R}([a,b])$, allora
$$
\inf_{x\in[a,b]} f(x)\le\frac{1}{b-a}\int_a^bf(x)dx\le\sup_{x\in[a,b]}f(x)
$$
inoltre se $f\in\mathcal{C}([a,b])$, allora esiste $c\in[a,b]:$
$$
f(c)=\frac{1}{b-a}\int_a^bf(x)dx
$$
# Dimostrazione
Sappiamo che
$$
\inf f(x)\le f(x)\sup f(x)
$$
allora per costruzione dell'integrale
$$
(b-a)\inf f(x)\le\int_a^bf(x)dx\le(b-a)\sup f(x)
$$
Sia ora $f\in\mathcal{C}([a,b])$, allora per [[Teorema dei valori intermedi]] esiste $c\in[a,b]:$
$$
f(c)=\frac{1}{b-a}\int_a^bf(x)dx\quad\square
$$