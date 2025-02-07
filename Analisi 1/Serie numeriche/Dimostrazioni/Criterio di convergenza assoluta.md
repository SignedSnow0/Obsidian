---
subject: analisi 1
type: dimostrazione
---
Se $\displaystyle\sum_{k=0}^\infty a_k$ converge assolutamente, allora $\displaystyle\sum_{k=0}^\infty a_k$ converge semplicemente, e $\displaystyle\left|\sum_{k=0}^\infty a_k\right|\le\sum_{k=0}^\infty |a_k|$
# Dimostrazione
Sia 
$$
a_k^+=\max\{a_k,0\},\quad a_k^-=\max\{-a_k,0\}
$$
allora le serie $\displaystyle\sum_{k=0}^\infty a_k^+,\sum_{k=0}^\infty a_k^-$ convergono per il teorema del confronto, e
$$
\left|\sum_{k=0}^\infty a_k\right|=\left|\sum_{k=0}^\infty(a_k^+-a_k^-)\right|\le\sum_{k=0}^\infty(a_k^++a_k^-)=\sum_{k=0}^\infty|a_k|\quad\square
$$