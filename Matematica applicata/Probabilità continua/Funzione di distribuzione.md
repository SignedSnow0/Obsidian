---
subject: matematica applicata
type: definizione
---
Sia $X$ una [[Variabile casuale|variabile casuale]], si dice funzione di distribuzione o ripartizione la funzione $F:\mathbb{R}\to[0,1]$ tale che
$$
F(x)=P(X\le x)
$$
Per più [[Variabile casuale|variabili casuali]] si estende la funzione $F:\mathbb{R}^n\to[0,1]$ tale che
$$
F(x_1,\dots,x_n)=P(X_1\le x_1\dots,X_n\le x_n)
$$
### Proprietà
1. $0\le F(x)\le 1$
2. $\displaystyle\lim_{x\to-\infty}F(x)=P(X\le-\infty)=0$
3. $\displaystyle\lim_{x\to+\infty}F(x)=P(X\le+\infty)=1$
4. Se $a<b$, allora $F(a)\le F(b)$, cioè $F$ non è mai decrescente
5. Se $X$ è una [[Variabile casuale|variabile casuale discreta]], allora $F$ è a gradini
6. Se $X$ è una [[Variabile casuale|variabile casuale continua]], allora $\displaystyle F(x)=\int_{-\infty}^xf(s)ds$ come visto nella [[Funzione densità|funzione densità]]

Usando il [[Principio di Cavalieri|principio di Cavalieri]] la distribuzione in più dimensioni può essere semplificato
$$
F_{x_j}(x_k)=P(X_k\le x_k)=P(X_j\le+\infty,X_k\le x_k)=F(x_k,+\infty)
$$