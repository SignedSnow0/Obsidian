Data una successione di [[Variabile casuale|v.c.]] $X_n$ [[Eventi indipendenti|i.]][[Funzione di distribuzione|i.d.]] con $\E[X]=\mu$, $\var(X)=\sigma^2$, allora la media aritmetica di tali variabili converge in probabilità al [[Valore atteso|valore atteso]] di ciascuna variabile:
$$
\lim_{n\to\infty}P(|\bar{X}-\mu|\ge\epsilon)=0\quad\forall\epsilon\in\mathbb{R}^+
$$
# Dimostrazione
Dato che $X_n$ sono [[Funzione di distribuzione|identicamente distribuite]]
$$
\E[X_1]=\dots=\E[X_n]=\mu
$$
$$
\var(X_1)=\dots=\var(X_n)=\sigma^2
$$
allora
$$
\E[\bar{X}]=\E\left[\frac{\sum_{k=1}^nX_k}{n}\right]=\frac{1}{n}\sum_{k=1}^n\E[X_k]=\frac{1}{n}\sum_{k=1}^n\mu=\frac{n\mu}{n}=\mu
$$
$$
\var(\bar{X})=\var\left(\frac{\sum_{k=1}^nX_k}{n}\right)=\frac{1}{n^2}\var\left(\sum_{k=1}^nX_k\right)=\frac{\sum_{k=1}^n\var(X_k)}{n^2}=\frac{\sum_{k=1}^n\sigma^2}{n^2}=\frac{n\sigma^2}{n^2}=\frac{\sigma^2}{n}
$$
allora per [[Disuguaglianza di Čebičev|Čebičev]]
$$
P(|\bar{X}-\mu|\ge\epsilon)\le\frac{\sigma^2}{n\epsilon^2}
$$
allora
$$
\lim_{n\to\infty}P(|\bar{X}-\mu|\ge\epsilon)\le\lim_{n\to\infty}\frac{\sigma^2}{n\epsilon^2}=0
$$
dagli [[Probabilità di Kolmogorov|assiomi]] $P(X)\ge0$, quindi
$$
\lim_{n\to\infty}P(|\bar{X}-\mu|\ge\epsilon)=0\quad\square
$$