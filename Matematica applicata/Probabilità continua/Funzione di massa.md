---
subject: matematica applicata
type: definizione
---
La funzione di massa è una funzione $p:\mathbb{R}\to[0,1]$ tale che 
$$
p(x)=P(X=x)
$$
dove $X$ è una [[Variabile casuale|variabile casuale]], e $x\in\mathbb{R}$.
Per più [[Variabile casuale|variabili casuali]] si estende la funzione $p:\mathbb{R}^n\to[0,1]$ tale che
$$
p(x_1,\dots,x_n)=P(X_1=x_1\dots,X_n=x_n)
$$
### Proprietà
1. $0\le p(x)\le 1$
2. $\displaystyle\sum_{j=1}^np(x_j)=P(S)=1$

Analogamente al [[Principio di Cavalieri|principio di Cavalieri]] possiamo ridurre la dimensione del problema
$$
p_{x_j}(x_k)=P(X_k=x_k,X_j\le+\infty)=\sum_{j=1}^np(x_k,x_j)
$$