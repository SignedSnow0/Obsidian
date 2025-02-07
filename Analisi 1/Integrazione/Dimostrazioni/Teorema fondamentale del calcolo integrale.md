---
subject: analisi 1
type: dimostrazione
---
Sia $f\in\mathcal{C}(I)$, sia 
$$
F_{x_0}(x)=\int_{x_0}^xf(s)ds
$$
allora $F$ è derivabile e si ha
$$
F_{x_0}'(x)=f(x)\quad\forall x\in I
$$
# Dimostrazione
Notiamo che
$$
\frac{F_{x_0}(x+h)-F_{x_0}(x)}{h}=\frac1h\left(\int_{x_0}^{x+h}f(s)ds-\int_{x_0}^xf(s)ds\right)=\frac1h\int_{x}^{x+h}f(s)ds
$$
Allora per [[Teorema della media integrale]] esiste $\displaystyle x_0\in[x,x+h]:f(x_0)=\frac1h\int_x^{x+h}f(s)ds$
Perciò, dato che se $h\to0\implies x_0=x$ abbiamo che
$$
\lim_{h\to 0}\frac{F_{x_0}(x+h)-F_{x_0}(x)}{h}=f(x)\quad\square
$$