Se il numero di [[Esito di un esperimento|esperimenti]] di evento $A$ tende all'infinito, la definizione [[Probabilità classica|frequentista]] di probabilità converge in probabilità [[Probabilità di Kolmogorov|teorica]] di $A$
$$
\lim_{n\to\infty}P(|f_A-p(A)|\ge\epsilon)=0\quad\forall\epsilon\in\mathbb{R}^+
$$
dove $f_A$ è la probabilità calcolata in maniera [[Probabilità frequentistica|frequentista]].
# Dimostrazione
Siano
$$
X_k=\begin{cases}0&\lnot A\\1&A\end{cases}
$$
allora
$$
\bar{X}=\sum_{k=1}^n\frac{X_k}{n}=f_A
$$
$$
\E[\bar{X}]=p
$$
allora per la [[Legge dei grandi numeri|legge dei grandi numeri]]
$$
\lim_{n\to+\infty}P(|\bar{X}-p|\ge\epsilon)=\lim_{n\to+\infty}P(|f_A-p(A)|\ge\epsilon)=0\quad\square
$$