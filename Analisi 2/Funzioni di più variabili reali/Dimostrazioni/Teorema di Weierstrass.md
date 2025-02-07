---
subject: analisi 2
type: dimostrazione
---
Sia $A\subseteq\mathbb{R}^n\ne\emptyset$ chiuso e limitato, $f:A\to\mathbb{R}^m,f\in\mathcal{C}$, allora
1. $f(A)\subseteq\mathbb{R}^m$ chiuso e limitato
2. se $m=1$, $f$ ammette minimo e massimo
# Dimostrazione
Sia *1.* valido, allora $f(A)\subseteq\mathbb{R}$, sia $r\in\mathbb{R}^+,m=\inf\{f(A)\}$, allora
$$
m-\frac{r}{2}\in I(m,r),\quad m-\frac{r}{2}\notin f(A)
$$
inoltre per definizione $m+r$ non è minorante di $f(A)$ per cui esiste $y\in f(A),y<m+r$ tale che
$$
m-r<m\le y
$$
perciò $y\in f(A)\cap I(m,r)$ e quindi ogni intorno circolare di $m$ contiene sia elementi did $f(A)$ che non e concludiamo che
$$
m\in\text{Fr}(f(A))\quad\square
$$

##### Correlati:
* [[Funzione continua]]