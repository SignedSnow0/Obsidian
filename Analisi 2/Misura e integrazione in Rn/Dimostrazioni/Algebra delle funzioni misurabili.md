---
subject: analisi 2
type: dimostrazione
---
Sia $A\in\mathcal{M}_n,f,g:A\to\mathbb{R}$ [[Funzione misurabile|misurabile]] $h:\mathbb{R}\to\mathbb{R}\in\mathcal{C},c\in\mathbb{R}$, allora
1. $f+g$ è misurabile
2. $fg,\frac fg$ è misurabile
3. $h\circ f$ è misurabile
4. $cf$ è misurabile
# Dimostrazione
Per definizione di [[Funzione misurabile|funzione misurabile]] esistono $\phi_k,\psi_k$ tali che
$$
\forall x\in A\quad\lim_{k\to+\infty}\phi_k(x)=f(x),\lim_{k\to+\infty}\psi_k(x)=g(x)
$$
per [[Algebra dei limiti|algebra dei limiti]]
$$
\lim_{k\to+\infty}(\phi_k(x)+\psi_k(x))=f(x)+g(x)
$$
$$
\lim_{k\to+\infty}(\phi_k(x)\psi_k(x))=f(x)g(x)
$$
inoltre
$$
\lim_{k\to+\infty}h(\phi_k)=h(f(x))
$$
e possiamo dire che $h\circ f$ è semplice prendendo partizioni di $A$ e $\alpha_1,\dots,\alpha_m:\phi_i=\alpha_i$, allora
$$
(h\circ f)(x)=h(\alpha_i)
$$
infine 4 deriva da 3 prendendo $h(y)=cy\quad\square$