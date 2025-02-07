---
subject: analisi 1
type: dimostrazione
---
Sia $x_0\in\mathbb{R}$ punto di accumulazione tale che $\displaystyle\lim_{x\to x_0}f(x)=l\in\overline{\mathbb{R}}$ e
* Se $l\in\mathbb{R}$, $g$ sia continua in $l$
* Se $l\in\{\pm\infty\}$, esista $\displaystyle\lim_{y\to l}g(y)$
Allora esiste il limite di $\displaystyle(g\circ f)(x)=\lim_{x\to x_0}g(f(x))=\lim_{y\to l}g(y)$.
# Dimostrazione
Sia $\displaystyle m=\lim_{y\to l}g(y)$
Allora per definizione di limite
$$
\forall I(m)\quad\exists J(l):g(y)\in I\quad\forall y\in J
$$
$$
\forall U(l)\quad\exists V(x_0):f(x)\in U\quad\forall x\in V
$$
Ma $U,J$ sono entrambi intorni di $l$, quindi possiamo scegliere $U=J$, allora
$$
\forall I(m)\quad\exists V(x_0):g(f(x))\in I\quad\forall x\in V
$$
Cioè $\displaystyle\lim_{x\to x_0}g(f(x))=m=\lim_{y\to l}g(y)\quad\square$