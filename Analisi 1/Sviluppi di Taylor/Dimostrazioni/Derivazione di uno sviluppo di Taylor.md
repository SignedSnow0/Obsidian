---
subject: analisi 1
type: dimostrazione
---
Sia $f$ n-volte derivabile in $x_0$, allora $\forall j\in\{0,\dots,n\}$ abbiamo
$$
(Tf_{n,x_0})^{(j)}(x)=Tf_{n-j,x_0}^{(j)}(x)
$$
# Dimostrazione
Iniziamo notando che
$$
\left((x-x_0)^k\right)^{(j)}=\begin{cases}\frac{k!}{(k-j)!}(x-x_0)^{k-j}\quad j\le k\\0\quad j>k\end{cases}
$$
allora
$$
(Tf_{n,x_0})^{(j)}(x)=\sum_{k=0}^{n}\frac{f^{k}(x_0)}{k!}\left((x-x_0)^k\right)^{(j)}=\sum_{k=0}^{n}\frac{f^{k}(x_0)}{k!}\frac{k!}{(k-j)!}(x-x_0)^{k-j}=\sum_{m=0}^{n-j}\frac{f^{(m+j)}(x_0)}{m!}(x-x_0)^m=Tf_{n-j,x_0}^{(j)}\quad\square
$$