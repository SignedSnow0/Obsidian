---
subject: analisi 2
type: dimostrazione
---
Sia $A\subseteq\mathbb{R}^n$ aperto, $B\subseteq\mathbb{R}^m$ aperto, $g\in\mathcal{C}^1(A),f\in\mathcal{C}^1(B;\mathbb{R}^n):f(B)\subseteq A$, allora:
1. $g\circ f\in\mathcal{C}^1(B)$
2. $$
D_i(g\circ f)(x)=\nabla g(f(x))\cdot D_if(x)=\sum_{j=1}^{n}\frac{\partial g}{\partial x_j}(f(x))\frac{\partial f_j}{\partial x_i}(x)
$$
# Dimostrazione
Sia $x\in B,\rho\in\mathbb{R}^+: B_n(f(x),\rho)\subseteq A$, poichè $f\in\mathcal{C}(B)$
$$
\exists\delta_1\in\mathbb{R}^+:y\in B_m(x,\delta_1)\implies f(y)\in B_n(f(x),\rho)
$$
Sia $i\in\{1,\dots,m\},t\in\mathbb{R}|t|<\delta_1$ si ha
$$
||(x+te^i)-x||_m=|t|<\delta_1
$$
perciò $x+te^i\in B,f(x+te^i)\in B_n(f(x),\rho)$ inoltre visto che $B_n(f(x),\rho)$ è convesso $[f(x),f(x+te^i)]$ è un segmento contenuto in $A$, allora per [[Teorema del valor medio]] esiste $z(t)\in[f(x),f(x+te^i)]:$
$$
g(f(x+te^i))-g(f(x))=\nabla g(z(t))\cdot(f(x+te^i))-f(x))
$$
inoltre per $t\ne 0$
$$
\frac{g(f(x+te^i))-g(f(x))}{t}=\nabla g(z(t))\cdot\frac{f(x+te^i))-f(x)}{t}=[\nabla g(f(x))+r(t)]\cdot[\frac{\partial f}{\partial x_i}(x)+s(t)]
$$
con
$$
r(t)=\nabla g(z(t))-\nabla g(f(x)),\quad s(t)=\frac{f(x+te^i)-f(x)}{t}-\frac{\partial f}{\partial x_i}(x)
$$
per la [[Disuguaglianza di Cauchy-Schwarz]]
$$
\left|\frac{g(f(x+te^i))-g(f(x))}{t}-\nabla g(f(x))\cdot\frac{\partial f}{\partial x_i}(x)\right|=
$$
$$
\left|r(t)\cdot\left[\frac{\partial f}{\partial x_i}(x)+s(t)\right]+[\nabla g(f(x))+r(t)]\cdot s(t)\right|\le
$$
$$
||r(t)||_n\left(\left|\left|\frac{\partial f}{\partial x_i}(x)\right|\right|_n+||s(t)||_n\right)+(||\nabla g(f(x))||_n+||r(t)||_n)||s(t)||_n
$$
Sia ora $\epsilon,\eta\in\mathbb{R}^+$, per definizione di derivata
$$
\exists\delta_2\in(0,\delta_1):|t|<\delta_2\implies||s(t)||_n<\eta
$$
poichè $g\in\mathcal{C}^1(A),\nabla g\in\mathcal{C}(A;\mathbb{R}^n)$
$$
\exists\delta_3\in(0,\rho):z\in\mathbb{R}^n,||z-f(x)||_n<\delta_3\implies||\nabla g(z)-\nabla g(f(x))||_n<\eta
$$
essendo $f\in\mathcal{C}(B)$
$$
\exists\delta_4\in(0,\delta_1):y\in\mathbb{R}^m,||y-x||_m<\delta_4\implies||f(y)-f(x)||_n<\delta_3
$$
Sia $|t|<\delta_4$ allora
$$
||(x+te^i)-x||_m<\delta_4\implies||f(x+te^i)-f(x)||_n<\delta_3
$$
infine essendo $z(t)\in[f(x),f(x+te^i)]$ si ha $||z(t)-f(x)||_n<\delta_3$, perciò 
$$
||r(t)||_n<\eta
$$
Perciò con $|t|<\max\{\delta_2,\delta_4\}$ otteniamo
$$
\left|\frac{g(f(x+te^i))-g(f(x))}{t}-\nabla g(f(x))\cdot\frac{\partial f}{\partial x_i}(x)\right|\le\eta\left(\left|\left|\frac{\partial f}{\partial x_i}(x)\right|\right|_n+||\nabla g(f(x))||_n+2\eta\right)
$$
scegliendo opportunamente $\eta$ in base ad $\epsilon$ otteniamo
$$
\left|\frac{g(f(x+te^i))-g(f(x))}{t}-\nabla g(f(x))\cdot\frac{\partial f}{\partial x_i}(x)\right|\le\epsilon\quad\square
$$