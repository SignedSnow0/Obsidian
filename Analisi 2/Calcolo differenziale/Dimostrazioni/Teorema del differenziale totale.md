---
subject: analisi 2
type: dimostrazione
---
Sia $A\subseteq\mathbb{R}^n,f\in\mathcal{C}^1(A),x\in A,v\in\mathbb{R}^n$, allora esiste $\frac{\partial f}{\partial v}(x)$ e
$$
\frac{\partial f}{\partial v}(x)=\nabla f(x)\cdot v=\sum_{j=1}^n\frac{\partial f}{\partial x_j}(x)v_j
$$
# Dimostrazione
Sia $n=2,A=\mathbb{R}^2,x=(x_1,x_2)\in\mathbb{R}^2,t\in\mathbb{R}\setminus\{0\},v=(v_1,v_2)$, allora
$$
f(x+tv)-f(x)=
$$
$$
(f(x_1+tv_1,x_2+tv_2)-f(x_1,x_2+tv2))+(f(x_1,x_2+tv_2)-f(x_1,x_2))
$$
sia $g:\mathbb{R}\to\mathbb{R},g(y)=f(y,x_2+tv_2)$, allora
$$
g'(y)=\frac{\partial f}{\partial y}(y,x_2+tv_2),\quad g\in\mathcal{C}^1(\mathbb{R})
$$
allora per [[Teorema dei valori intermedi]]
$$
\exists c_1(t)\in[x_1,x_1+tv_1]:f(x_1+tv_1,x_2+tv_2)-f(x_1,x_2+tv_2)=
$$
$$
g(x_1+tv_1)-g(x_1)=g'(c_1(t))tv_1=\frac{\partial f}{\partial c_1(t)}(c_1(t),x_2+tv_2)tv_1
$$
analogamente per $c_2(t)$
$$
f(x_1,x_2+tv_2)-f(x_1,x_2)=\frac{\partial f}{\partial c_2(t)}(x_1,c_2(t))tv_2
$$
segue allora
$$
\frac{f(x+tv)-f(x)}{t}=\frac{\partial f}{\partial c_1(t)}(c_1(t),x_2+tv_2)v_1+\frac{\partial f}{\partial c_2(t)}(x_1,c_2(t))tv_2
$$
siano $\epsilon\eta\in\mathbb{R}^+$, poichè $\frac{\partial f}{\partial c_1(t)},\frac{\partial f}{\partial c_2(t)}\in\mathcal{C}$
$$
\exists\delta(\eta)\in\mathbb{R}^+:||z-x||<\delta(\eta)\implies\left|\frac{\partial f}{\partial c_j(t)}(z)-\frac{\partial f}{\partial c_j(t)}(x)\right|<\eta
$$
inoltre
$$
||C_1(t),x_2+tv_2)-x||=\sqrt{(c_1(t)-x_1)^2+t^2v^2}=\sqrt{t^2(v_1^2+v_2^2)}=|t|||v||
$$
e
$$
||x_1,c_2(t))-x||=|c_2(t)-x_2|\le|t||v_2|
$$
sia ora $\delta_2(\eta)\in\mathbb{R}^+:t\in\mathbb{R}\setminus\{0\},|t|<\delta_2(\eta)\implies$
$$
|t|||v||<\delta_1(\eta)
$$
allora
$$
\left|\frac{f(x+tv)-f(x)}{t}-\frac{\partial f}{\partial c_1(t)}(x)v_1-\frac{\partial f}{\partial c_2(t)}(x)v_2\right|\le\eta(|v_1|+|v_2|)
$$
scegliendo $\eta:\eta(|v_1|+|v_2|)<\epsilon$
$$
\left|\frac{f(x+tv)-f(x)}{t}-\frac{\partial f}{\partial c_1(t)}(x)v_1-\frac{\partial f}{\partial c_2(t)}(x)v_2\right|<\epsilon\quad\square
$$