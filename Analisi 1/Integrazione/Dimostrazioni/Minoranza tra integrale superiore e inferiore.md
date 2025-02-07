---
subject: analisi 1
type: dimostrazione
---
Sia $f$ limitata su $[a,b]$, allora
$$
\underline{\int_I}f\le\overline{\int_I}f
$$
# Dimostrazione
Sia $g\in\mathcal{S}_f^-,h\in\mathcal{S}_f^+$, allora per [[Minoranza di integrali su funzioni a scala]]
$$
\int_Ig\le\int_Ih
$$
Scegliendo $h=\inf\{S_f^+\}$
$$
\int_Ig\le\overline{\int_I}f
$$
Scegliendo $g=\sup\{S_f^-\}$
$$
\underline{\int_I}f\le\overline{\int_I}f\quad\square
$$