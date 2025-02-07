Data una [[Variabile casuale|v.c.]] $X$ a valori non negativi e un valore $a\in\mathbb{R}^+$, allora
$$
P(X\ge a)\le\frac{\E[x]}{a}
$$
# Dimostrazione
Dato che $X$ è non negativa
$$
\E[X]=\int_\mathbb{R}xf(x)dx=\int_0^{+\infty}xf(x)dx=\int_0^axf(x)dx+\int_a^{+\infty}xf(x)dx\ge\int_a^{+\infty}xf(x)dx\ge
$$
dato che nel secondo integrale $x\ge a$
$$
\ge\int_a^{+\infty}af(x)dx=a\int_a^{+\infty}f(x)dx=aP(X\ge a)
$$
allora
$$
\E[X]\ge aP(X\ge a)\quad\square
$$