---
subject: analisi 1
type: dimostrazione
---
Sia $f:[a,b]\to\mathbb{R}$, allora $f\in\mathcal{R}([a,b])\iff\forall\epsilon>0\quad\exists h_\epsilon\in S_f^+,g_\epsilon\in S_f^-:$
$$
\int_a^bh_\epsilon(x)dx-\int_a^bg_\epsilon(x)dx<\epsilon
$$
# Dimostrazione
Sia $f\in\mathcal{R}([a,b])$, allora esiste
$$
\underline{\int_{[a,b]}}f(x)dx,\quad\overline{\int_{[a,b]}}f(x)dx
$$
Scegliamo perciò $h_\epsilon,g_\epsilon$ tali che
$$
\int_{[a,b]}h_\epsilon(x)dx-\overline{\int_{[a,b]}}f(x)dx<\frac\epsilon2,\quad\underline{\int_{[a,b]}}f(x)dx-\int_{[a,b]}g_\epsilon(x)dx<\frac\epsilon2
$$
allora
$$
\int_{[a,b]}h_\epsilon(x)dx-\int_{[a,b]}g_\epsilon(x)dx<\epsilon
$$
Invece, se vale la seconda ipotesi abbiamo che
$$
\int_{[a,b]}g_\epsilon(x)dx\le\underline{\int_{[a,b]}}f(x)dx\le\overline{\int_{[a,b]}}f(x)dx\le\int_{[a,b]}h_\epsilon(x)dx
$$
quindi
$$
\overline{\int_{[a,b]}}f(x)dx-\underline{\int_{[a,b]}}f(x)dx<\epsilon\quad\square
$$