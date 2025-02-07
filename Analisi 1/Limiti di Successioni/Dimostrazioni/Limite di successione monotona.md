---
subject: analisi 1
type: dimostrazione
---
Sia $a_n$ monotona crescente, allora
* Se $a_n$ è limitata $\displaystyle\lim_{n\to\infty}a_n=\sup\{a_n\}$
* Se $a_n$ non è limitata $\displaystyle\lim_{n\to\infty}=\infty$
# Dimostrazione
* Caso limitato:
Sia $l=\sup\{a_n\}$, per definizione di limite:
$$
\forall\epsilon>0\quad\exists n_\epsilon:l-\epsilon<a_n<l+\epsilon\quad\forall n\ge n_\epsilon
$$
Inoltre $a_{n_\epsilon}<a_n\quad\forall n\ge n_\epsilon$, unendo le tre proposizioni:
$$
l-\epsilon<a_{n_\epsilon}\le a_n\le l<l+\epsilon
$$
* Caso non limitato:
Sia $l=\infty$, per definizione di limite:
$$
\forall M>0\quad\exists n_M:a_n>M\quad\forall n\ge n_M
$$
Inoltre $a_n\ge a_{n_M}\quad\forall n\ge n_M$, perciò
$$
M<a_{n_M}\le a_n\quad\square
$$