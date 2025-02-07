---
subject: analisi 1
type: dimostrazione
---
Sia $f$ n-volte derivabile in $x_0$ con $f^{(n)}\in\mathcal{C^1}(x_0)$ allora
$$
f(x)=Tf_{n,x_0}(x)+\frac{f^{(n+1)}(\overline{x})}{(n+1)!}(x-x_0)^{n+1}\quad\forall x\in I_r(x_0)\setminus\{x_0\}
$$
per un $\overline{x}\in(x_0,x)$
# Dimostrazione
Dimostriamo che 
$$
\frac{f(x)-Tf_{n,x_0}(x)}{(x-x_0)^{n+1}}=\frac{f^{(n+1)}(\overline{x})}{(n+1)!}
$$
Siano
$$
\phi(x)=f(x)-Tf_{n,x_0}(x),\quad\psi(x)=(x-x_0)^{n+1}
$$
Sappiamo che $\phi^{(j)}(x_0)=0\quad\psi^{(j)}(x_0)=0\quad\forall j\in\{0,\dots,n\}$, allora per [[Teorema di Cauchy]]
$$
\frac{\phi(x)}{\psi(x)}=\frac{\phi(x)-\phi(x_0)}{\psi(x)-\psi(x_0)}=\frac{\phi'(x_1)}{\psi'(x_1)}
$$
Iterando otteniamo
$$
\frac{\phi(x)}{\psi(x)}=\dots=\frac{\phi^{(n+1)}(x_{n+1})}{\psi^{(n+1)}(x_{n+1})}=\frac{f^{(n+1)}(x_{n+1})}{(n+1)}\quad\square
$$