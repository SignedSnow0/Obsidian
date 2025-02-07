---
subject: analisi 1
type: dimostrazione
---
Sia $f\in\mathcal{C}([a,b])$, limitata in $(a,b)$, allora $f\in\mathcal{R}([a,b])$
# Dimostrazione
Notiamo che $f\in\mathcal{R}([a+\epsilon,b-\epsilon])$, sia ora $\phi_\epsilon,\psi_\epsilon\in\mathcal{S}([a+\epsilon,b-\epsilon])$ tali che
$$
\phi_\epsilon(x)\le\psi_\epsilon(x)\quad\forall x\in[a+\epsilon,b-\epsilon],\quad\int_a^b\psi_\epsilon(x)dx-\int_a^b\phi_\epsilon(x)<\epsilon
$$
Siano ora
$$
h_\epsilon=\begin{cases}\psi_\epsilon(x)\quad x\in[a+\epsilon,b-\epsilon]\\\sup f(x)\quad x\in[a,b]\setminus[a+\epsilon,b-\epsilon]\end{cases}
$$
$$
g_\epsilon=\begin{cases}\phi_\epsilon(x)\quad x\in[a+\epsilon,b-\epsilon]\\\inf f(x)\quad x\in[a,b]\setminus[a+\epsilon,b-\epsilon]\end{cases}
$$
Allora
$$
\int_a^bh_\epsilon(x)dx-\int_a^bg_\epsilon(x)dx=\int_a^{a+\epsilon}(h_\epsilon-g_\epsilon)(x)dx+\int_{a+\epsilon}^{b-\epsilon}(\psi_\epsilon-\phi_\epsilon)(x)dx+\int_{b-\epsilon}^b(h_\epsilon-g_\epsilon)(x)dx\le2(\sup f(x)-\inf f(x))\epsilon+\epsilon
$$
che soddisfa [[Integrale secondo Riemann]] $\square$