Data una [[Variabile casuale|v.c.]] $X$ e un numero $r\in\mathbb{R}^+$, allora
$$
P(|X-\mu|\ge r)\le\frac{\sigma^2}{r^2}
$$
# Dimostrazione
$$
P(|X-\mu|\ge r)=P((X-\mu)^2\ge r^2)
$$
per [[Disuguaglianza di Markov|Markov]] 
$$
P((X-\mu)^2\ge r^2)=P(Y\ge r^2)\le\frac{\E[Y]}{r^2}=\frac{\E[(X-\mu)^2]}{r^2}=\frac{\var(X)}{r^2}
$$
allora 
$$
P(|X-\mu|\ge r)\le\frac{\var(X)}{r^2}=\frac{\sigma^2}{r^2}\quad\square
$$