---
subject: analisi 2
type: teorema
---
Notiamo attraverso l'enunciato di alcuni teoremi che nel caso unidimensionale l'[[Integrale di Lebesgue per funzione sommabile|integrale di Lebesgue]] è un estensione dell'[[Integrale di Riemann|integrale di Riemann]].
## Teorema 1
Sia $a,b\in\mathbb{R},a<b,f:[a,b]\to\mathbb{R}\in\mathcal{R}$, allora $f$ è sommabile e l'[[Integrale di Lebesgue per funzione sommabile|integrale di Lebesgue]] coincide con [[Integrale di Riemann]].

## Teorema 2
Sia $-\infty<a<b\le+\infty,f:[a,b]\to\mathbb{R}$ non negativa e integrabile secondo Riemann per ogni $[a,c],a<c<b$, allora
1. $\displaystyle\exists\lim_{c\to b}\int_a^cf(x)dx$
2. $f$ è [[Funzione misurabile|misurabile]] e $\displaystyle\int_{[a,b)}f(x)dx=\lim_{c\to b}\int_a^cf(x)dx$

## Teorema 3
Sia $-\infty\le a<bz<+\infty,f:[a,b]\to\mathbb{R}$ non negativa e integrabile secondo Riemann per ogni $[a,c],a<c<b$, allora
1. $\displaystyle\exists\lim_{c\to a}\int_c^bf(x)dx$
2. $f$ è [[Funzione misurabile|misurabile]] e $\displaystyle\int_{(a,b]}f(x)dx=\lim_{c\to a}\int_c^bf(x)dx$

## Teorema 4
Sia $-\infty<a<b\le+\infty,f:[a,b)\to\mathbb{R}\in\mathcal{R}$ in ogni intervallo $[a,c]$, supponiamo esista $\displaystyle\lim_{c\to b}\int_a^c|f(x)|dx$, allora
1. $f$ è [[Funzione sommabile|sommabile]] in $[a,b)$
2. $\displaystyle\exists\lim_{c\to b}\int_a^cf(x)dx\in\mathbb{R}$
3. $\displaystyle\int_{[a,b)}f(x)dx=\lim_{c\to b}f(x)dx$