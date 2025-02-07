---
subject: analisi 1
type: dimostrazione
---
Sia $x_0\in\mathring D,f,g$ derivabili in $x_0$, allora 
* $(f\pm g)'(x)=f'(x_0)\pm g'(x_0)$
* $(fg)'(x)=f'(x_0)g(x_0)+f(x_0)g'(x_0)$
* $\left(\frac fg\right)'(x)=\frac{f'(x_0)g(x_0)-f(x_0)g'(x_0)}{g^2(x_0)}$
# Dimostrazione
Iniziamo osservando che
$$
f(x)g(x)-f(x_0)g(x_0)=f(x)g(x)-f(x_0)g(x)+f(x_0)g(x)-f(x_0)g(x_0)=(f(x)-f(x_0))g(x)+f(x_0)(g(x)-g(x_0))
$$
Allora prendendo il rapporto incrementale
$$
\lim_{x\to x_0}\frac{f(x)-f(x_0)}{x-x_0}g(x)+f(x_0)\lim_{x\to x_0}\frac{g(x)-g(x_0)}{x-x_0}=f'(x_0)g(x_0)+f(x_0)g'(x_0)
$$
Per il rapporto osserviamo che
$$
\frac{f(x)}{g(x)}-\frac{f(x_0)}{g(x_0)}=\frac{f(x)}{g(x)}-\frac{f(x_0)}{g(x)}+\frac{f(x_0)}{g(x)}-\frac{f(x_0)}{g(x_0)}=\frac{f(x)-f(x_0)}{g(x)}+\frac{f(x_0)(g(x_0)-g(x))}{g(x_0)g(x)}
$$
Sempre prendendo il rapporto incrementale abbiamo
$$
\lim_{x\to x_0}\frac{f(x)-f(x_0)}{x-x_0}\frac1{g(x)}+f(x_0)\lim_{x\to x_0}\frac{g(x_0)-g(x)}{x-x_0}\frac1{g(x)g(x_0)}=\frac{f'(x_0)}{g(x_0)}-\frac{f(x_0)g'(x_0)}{g^2(x_0)}=\frac{f'(x_0)g(x_0)-f(x_0)g'(x_0)}{g^2(x_0)}\quad\square
$$