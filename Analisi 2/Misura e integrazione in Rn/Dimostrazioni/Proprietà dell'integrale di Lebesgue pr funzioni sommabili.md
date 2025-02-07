---
subject: analisi 2
type: dimostrazione
---
Sia $A\in\mathcal{M}_n,f,g:A\to\mathbb{R}$  [[Funzione misurabile|misurabili]] non negative, allora:
1. $\displaystyle\int_Af(x)dx\in[0,+\infty]$
2. se $f(x)\le g(x)\quad\forall x\in A$, allora $\displaystyle\int_Af(x)dx\le\int_Ag(x)dx$
3. $\displaystyle\int_A(f+g)(x)dx=\int_Af(x)dx+\int_Ag(x)dx$
4. se $\alpha\in[0,+\infty)$
$$
\int_A\alpha f(x)dx=\alpha\int_Af(x)dx
$$
5. se $A=A_1\cup\dots\cup A_p$ misurabili e disgiunti
$$
\int_Af(x)dx=\sum_{i=1}^{p}\int_{A_i}f(x)dx
$$
con $\displaystyle\int_{A_i}f(x)dx=\int_{A_i}f_{|A_i}(x)dx$
# Dimostrazione
1 segue dalla definizione di [[Integrale di Lebesgue per funzione misurabile|integrale]] e 
[[Proprietà dell'integrale di Lebesgue per funzioni semplici|proprietà degli integrali]].
Sia $\phi:A\to\mathbb{R}$ [[Funzione semplice|semplice]], $0\le\phi(x)\le f(x)\quad\forall x\in A$, allora $0\le\phi(x)\le g(x)\quad\forall x\in A$
$$
\int_A\phi(x)dx\le\int_Ag(x)dx
$$
e per definizione
$$
\int_Af(x)dx\le\int_Ag(x)dx\quad\square
$$