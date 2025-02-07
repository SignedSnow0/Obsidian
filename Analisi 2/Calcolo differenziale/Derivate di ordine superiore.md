---
subject: analisi 2
type: definizione
---
Sia $A\subseteq\mathbb{R}^n,f:A\to\mathbb{R}$, sia
$$
A_j=\left\{x\in A\space|\space\exists \frac{\partial f}{\partial x_j}(x)\in\mathbb{R}\right\}
$$
Allora a partire da questo insieme definiamo la derivata seconda $\frac{\partial f}{\partial x_i}(\frac{\partial f}{\partial x_j})(x)$ di $\frac{\partial f}{\partial x_j}$ in $x$ rispetto alle variabili $x_i,x_j$ e viene indicata come
$$
D_{ij}f(x)\quad\frac{\partial^2f}{\partial x_i\partial x_j}(x)
$$
oppure se $j=i$
$$
D_j^2f(x)\quad\frac{\partial^2f}{\partial x_j^2}(x)
$$
Infine iterando il procedimento otteniamo in generale
$$
D_{j_1\dots j_k}f(x)=D_{j_1}(\dots(D_{j_k}f)\dots)(x)=\frac{\partial^k f}{\partial x_{j_1}\dots\partial x_{j_k}}(x)
$$