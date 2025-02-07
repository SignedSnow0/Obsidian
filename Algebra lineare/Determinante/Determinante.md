---
subject: algebra lineare
type: definizione
---
Nella sua forma più astratta il determinante è una funzione
$$
\det:\mathbb{R}^{n,n}\to\mathbb{R}
$$
tale che se la matrice non ha [[Rango|rango]] massimo si annulla
$$
\forall A\in\mathbb{R}^{n,n}\quad\det A=0\iff \text{r}(A)\ne n
$$
Una definizione più utile per il calcolo del suo valore è la seguente:

Sia $A\in\mathbb{R}^{n,n},A=(a_{ij})$, allora:
1. se $n=1,\quad\det A=a_{11}$
2. se $\displaystyle n\ge 2\quad\det A=\sum_{j=1}^na_{1j}\mathcal{A}_{1j}$

dove $\mathcal{A}_{1j}$ è il [[Complemento algebrico|complemento algebrico]] ottenuto eliminando la prima riga e la $j$-esima colonna.