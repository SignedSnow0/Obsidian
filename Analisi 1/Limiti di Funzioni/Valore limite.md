Sia $f:D\to\mathbb{R},x_0\in\overline{\mathbb{R}}$ [[Analisi 1/Limiti di Funzioni/Punto di accumulazione|punto di accumulazione]] per $D$, diremo che $L\in\overline{\mathbb{R}}$ è un valore limite di $f$ per $x$ che tende a $x_0$ se per ogni $U$ [[Intorno di un punto|intorno]] di $L$ esiste $W$ [[Intorno di un punto|intorno]] di $x_0$ tale che
$$
f(W\cap (D\setminus\{x_0\}))\subset U
$$
La seguente definizione diventa, a seconda dei casi:
* $\forall\epsilon>0\quad\exists\delta>0:\forall x\in D\setminus\{x_0\},|x-x_0|<\delta\implies|f(x)-L|<\epsilon$ se $x_0,L\in\mathbb{R}$
* $\forall\epsilon>0\quad\exists c\in\mathbb{R}:\forall x>c\implies|f(x)-L|<\epsilon$ se $x_0=+\infty,L\in\mathbb{R}$
* $\forall\epsilon>0\quad\exists c\in\mathbb{R}:\forall x<c\implies|f(x)-L|<\epsilon$ per $x_0=-\infty,L\in\mathbb{R}$
* $\forall c\in\mathbb{R}\quad\exists\delta>0:\forall x\in D\setminus\{x_0\}:|x-x_0|<\delta\implies f(x)>c$ se $x_0\in\mathbb{R},L=+\infty$
* $\forall c\in\mathbb{R}\quad\exists\delta>0:\forall x\in D\setminus\{x_0\}:|x-x_0|<\delta\implies f(x)<c$ se $x_0\in\mathbb{R},L=-\infty$
* $\forall c\in\mathbb{R}\quad\exists d\in\mathbb{R}:\forall x>d\implies f(x)>c$ se $x_0=+\infty,L=+\infty$
* $\forall c\in\mathbb{R}\quad\exists d\in\mathbb{R}:\forall x<d\implies f(x)>c$ se $x_0=-\infty,L=+\infty$
* $\forall c\in\mathbb{R}\quad\exists d\in\mathbb{R}:\forall x>d\implies f(x)<c$ se $x_0=+\infty,L=-\infty$
* $\forall c\in\mathbb{R}\quad\exists d\in\mathbb{R}:\forall x<d\implies f(x)<c$ se $x_0=-\infty,L=-\infty$