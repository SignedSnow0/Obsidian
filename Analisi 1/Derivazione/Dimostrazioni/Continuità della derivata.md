---
subject: analisi 1
type: dimostrazione
---
Sia $x_0\in\mathring D,f$ continua in $x_0$, derivabile in $I_r(x_0)\setminus\{x_0\}$, se esiste $\displaystyle\lim_{x\to x_0}f'(x)\in\mathbb{R}$, allora $f$ è derivabile in $x_0$ e $f'$ è continua in $x_0$, cioè $\displaystyle f'(x_0)=\lim_{x\to x_0}f'(x)$
# Dimostrazione
Sia $h(x)=f(x)-f(x_0),\quad g(x)=x-x_0$, allora per de l'Hopital
$$
f'(x_0)=\lim_{x\to x_0}\frac{f(x)-f(x_0)}{x-x_0}=\lim_{x\to x_0}f'(x)\quad\square
$$