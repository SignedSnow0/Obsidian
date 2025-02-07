Sia $L\in\overline{\mathbb{R}}$, allora $\displaystyle\lim_{x\to x_0}f(x)=L$ se e solo se per ogni successione $a_n:\mathbb{N}\to D\setminus\{x_0\}$ tale che $\displaystyle\lim_{n\to+\infty}a_n=x_0$ abbiamo $\displaystyle\lim_{n\to+\infty}f(a_n)=L$

## Dimostrazione
Dalla definizione di [[Valore limite|limite]] abbiamo che se $\displaystyle\lim_{x\to x_0}f(x)=L\in\overline{\mathbb{R}}$, allora per ogni [[Intorno di un punto|intorno]] $U$ di $L$ esiste un intorno $W$ di $x_0$ tale che 
$$
f(W\cap (D\setminus\{x_0\}))\subset U
$$
Allora prendendo una successione $a_n:\mathbb{N}\to D\setminus\{x_0\}$ tale che $a_n\to x_0$ avremo che $a_n\in W\cap(D\setminus\{x_0\})$ [[Definitivamente|definitivamente]], ma ciò implica che $f(a_n)\in U$ [[Definitivamente|definitivamente]], perciò concluderemo che $f(a_n)\to L$
Supponiamo per assurdo che $L$ non sia limite di $f$ per $x\to x_0$, allora esiste un [[Intorno di un punto|intorno]] $U$ di $L$ tale che per ogni $W$ [[Intorno di un punto|intorno]] di $x_0$ esiste $a_n\in W\cap(D\setminus\{x_0\})$ tale che $f(a_n)\notin U$, allora ciò varrà per ogni intervallo
* $W_n=\left(x_0-\frac{1}{n+1},x_0+\frac{1}{n+1}\right)$ se $x_0\in\mathbb{R}$
* $W_n=(n,+\infty)$ se $x_0=+\infty$
* $W_n=(-\infty,-n)$ se $x_0=-\infty$

Dunque costruendo una successione $a_n$ prendendo $a_n\in W_n\cap(D\setminus\{x_0\})$ si avrà che $f(a_n)\notin U$ e quindi $f(a_n)$ non tende ad $L$ in contraddizione con il primo punto.