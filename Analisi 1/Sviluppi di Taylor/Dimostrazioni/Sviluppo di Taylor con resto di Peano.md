---
subject: analisi 1
type: dimostrazione
---
Sia $f$ n-volte derivabile in $x_0$, allora
$$
f(x)=Tf_{n,x_0}(x)+o((x-x_0)^n)
$$
# Dimostrazione
Iniziamo notando che
$$
\lim_{x\to x_0}\frac{f(x)-Tf_{n,x_0}(x)}{(x-x_0)^n}=\left[\frac00\right]
$$
Per il Teorema di de l'Hopital e [[Derivazione di uno sviluppo di Taylor]] abbiamo che
$$
\lim_{x\to x_0}\frac{f(x)-Tf_{n,x_0}(x)}{(x-x_0)^n}=\dots=\lim_{x\to x_0}\frac{f^{(n+1)}(x)-Tf_{1,x_0}^{(n-1)}}{n!(x-x_0)}=
$$
$$
= \frac1{n!}\lim_{x\to x_0}\frac{f^{(n-1)}(x)-f^{(n-1)}(x_0)-f^{(n)}(x_0)(x-x_0)}{x-x_0}=\frac{1}{n!}\lim_{x\to x_0}\left(\frac{f^{(n-1)}(x)-f^{(n-1)}(x_0)}{x-x_0}-f^{(n)}(x_0)\right)=0\quad\square
$$