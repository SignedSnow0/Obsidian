---
subject: analisi 2
type: dimostrazione
---
1. ogni intervallo n-dimensionale appartiene a $\mathcal{M}_n$
2. ogni sottoinsieme aperto di $\mathbb{R}^n$ appartiene a $\mathcal{M}_n$
3. ogni sottoinsieme chiuso di $\mathbb{R}^n$ appartiene a $\mathcal{M}_n$
4. se $A\subseteq\mathbb{R}^n, L_n(A)=0$ allora $A\in\mathcal{M}_n$
# Dimostrazione
Sia $E\subseteq\mathbb{R}^n$, per [[Proprietà della misura esterna]]
$$
0\le L_n^*(E\cap A)\le L_n^*(A)=0
$$
ne segue che 
$$
L_n^*(E\cap A)+L_n^*(E\cap A^c)=L_n^*(E\cap A^c)\le L_n^*(E)
$$