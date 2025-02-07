---
subject: analisi 2
type: teorema
---
Sia $\Omega\subseteq\mathbb{R}^n$ aperto, $T:\Omega\to\mathbb{R}^n$ [[Cambiamento di variabile|cambiamento di variabile]], $A\in\mathcal{M}_n,f:A\to\mathbb{R}, A\subseteq T(\Omega)$, allora
1. $T^{-1}(A)\in\mathcal{M}_n$
2. $f$ è [[Funzione integrabile|integrabile]] su $A\iff f(T(x))|\det J_T(x)|$ è [[Funzione integrabile|integrabile]] su $T^{-1}(A)$
3. $$
\int_Af(y)dy=\int_{T^{-1}(A)}f(T(x))|\det J_T(x)|dx
$$