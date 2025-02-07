---
subject: analisi 1
type: dimostrazione
---
Sia $a_n\le b_n\le c_n$ definitivamente, se $a_n\to l,c_n\to l$, allora $b_n\to l$
# Dimostrazione
Per definizione di limite
$$
\forall\epsilon>0\quad\exists \tilde{n_\epsilon}:|a_n-l|<\epsilon\quad\forall n\ge\tilde{n_\epsilon}
$$
$$
\forall\epsilon>0\quad\exists \bar{n_\epsilon}:|c_n-l|<\epsilon\quad\forall n\ge\bar{n_\epsilon}
$$
Sia ora $n_\epsilon=\max\{\tilde{n_\epsilon}\bar{n_\epsilon}\}$, allora
$$
\forall\epsilon>0\quad\exists n_\epsilon:l-\epsilon<a_n\le b_n\le c_n<l+\epsilon\quad\forall n\ge n_\epsilon\quad\square
$$