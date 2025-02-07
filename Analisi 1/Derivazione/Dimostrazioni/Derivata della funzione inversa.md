---
subject: analisi 1
type: dimostrazione
---
Sia $x_0\in\mathring{D},f$ derivabile in $x_0,f'(x_0)\ne0$, allora $f^{-1}$ è derivabile in $y_0=f(x_0)$ e $(f^{-1})'(y_0)=\frac{1}{f'(x_0)}=\frac{1}{f'(f^{-1}(y_0))}$
# Dimostrazione
Notiamo che
$$
\frac{f^{-1}(y)-f^{-1}(y_0)}{y-y_0}=\frac{x-x_0}{f(x)-f(x_0)}
$$
allora
$$
\lim_{x\to x_0}\frac{x-x_0}{f(x)-f(x_0)}=\lim_{x\to x_0}\frac{1}{\frac{f(x)-f(x_0)}{x-x_0}}=\frac{1}{f'(x_0)}\quad\square
$$