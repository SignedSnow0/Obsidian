---
subject: analisi 1
type: dimostrazione
---
Sia $\{a_n\}:a_n\to\lambda,\quad a_n\to\gamma$, allora $\lambda=\gamma$
# Dimostrazione
Per definizione di limite abbiamo che
$$
\forall\epsilon>0\quad\exists \bar{n_\epsilon}:|a_n-\lambda|<\epsilon\quad\forall n\ge\bar{n_\epsilon}
$$
$$
\forall\epsilon>0\quad\exists \tilde{n_\epsilon}:|a_n-\gamma|<\epsilon\quad\forall n\ge\tilde{n_\epsilon}
$$
Scegliendo $n_\epsilon=\max\{\bar{n_\epsilon},\tilde{n_\epsilon}\}$, entrambe le condizioni si avverano, quindi
$$
|\lambda-\gamma|=|\lambda-a_n+a_n-\gamma|\le|a_n-\lambda|+|a_n-\gamma|<2\epsilon\quad\square
$$