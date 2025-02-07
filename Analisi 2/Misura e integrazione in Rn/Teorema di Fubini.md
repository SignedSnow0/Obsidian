---
subject: analisi 2
type: teorema
---
Sia $A\in\mathcal{M}_{m+n},f:A\to\mathbb{R}$ [[Funzione sommabile|sommabile]], $B\in\mathcal{M}_m$ tale che 
$$
\{x\in\mathbb{R}^m|A_x\in\mathcal{M}_n,L_n(A_x)>0\}\subseteq B
$$
definiamo 
$$
g:B\to\mathbb{R},g(x)=\begin{cases}\displaystyle\int_{A_x}f(x,y)dy\quad A_x\in\mathcal{M}_n,f(x,.)\text{ è sommabile in }A_x\\0\end{cases}
$$
allora $g$ è misurabile e 
$$
\int_Bg(x)dx=\int_Af(x,y)dxdy=\int_B\left(\int_{A_x}f(x,y)dy\right)dx
$$

##### Correlati:
* [[Insieme misurabile]]