---
subject: analisi 1
type: dimostrazione
---
Sia $\displaystyle m_k=\min_{x\in I_k}{f(x)},\quad M_k=\max_{x\in I_k}{f(x)},\quad \Delta x=\frac{b-a}{n}$, allora le successioni
$$
s_n=\sum_{k=1}^{n}m_k\Delta x,\quad S_n=\sum_{k=1}^{n}M_k\Delta x
$$
convergono allo  stesso limite e poniamo l'integrale definito come
$$
\int_a^bf(x)dx=\lim_{n\to\infty}s_n=\lim_{n\to\infty}S_n
$$
# Dimostrazione
Iniziamo osservando che $\forall m\ge1$
$$
s_n\le s_{mn},\quad S_n\ge S_{mn}
$$
Poniamo $s=\sup{s_n},\quad S=\inf{S_n}$, allora sappiamo che $s<S$.
Dato che la funzione è continua sappiamo che $\forall\epsilon>0\quad\exists\delta>0:|x'-x''|<\delta\implies|f(x')-f(x'')|<\epsilon$ per qualche $x',x''\in[a,b]$, sia allora $n_\epsilon:\frac{b-a}{n_\epsilon}<\delta$.
Inoltre prendiamo per ogni intervallo $I_k$
$$
\xi_k:f(\xi_k)=\min_{x\in I_k}{f(x)}=m_k,\quad\eta_k:f(\eta_k)=\max_{x\in I_k}{f(x)}=M_k
$$
Allora dato che $|\eta_k-\xi_k|<\delta\implies M_k-m_k<\epsilon$, infine sommando ogni intervallo abbiamo che
$$
S_n-s_n=\sum_{k=1}^{n}{(M_k-m_k)}\Delta x<\epsilon\sum_{k=1}^{n}{\Delta x}=\epsilon(b-a)
$$
cioè $\forall\epsilon>0\quad\exists n_\epsilon:S-s<\epsilon\quad\forall n\ge n_\epsilon\quad\square$