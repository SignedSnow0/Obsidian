---
subject: analisi 2
type: dimostrazione
---
1. $\emptyset\in\mathcal{M}_n$
2. $A\in\mathcal{M}_n\implies A^c\in\mathcal{M}_n$
3. Sia $a_k$ una successione, allora $\displaystyle\bigcup_{k\in\mathbb{N}}a_k\in\mathcal{M}_n$
4. $L_n(\emptyset)=0$
5. $\displaystyle L_n\left(\bigcup_{k\in\mathbb{N}}a_k\right)=\sum_{k=1}^{\infty}L_n(a_k)$

Perciò $\mathcal{M}_n$ è una [[σ-algebra]] e $L_n$ è la sua misura.
# Dimostrazione
Dimostriamo il punto uno, si ha
$$
L_n^*(E\cap\emptyset)+L_n^*(E\cap\emptyset^c)=L_n^*(\emptyset)+L_n^*(E\cap\mathbb{R}^n)=L_n^*(E)
$$
Dimostriamo ora il punto due:
$$
L_n^*(E\cap A^c)+L_n^*(E\cap (A^c)^c)=L_n^*(E\cap A^c)+L_n^*(E\cap A)=L_n^*(E)\quad\square
$$