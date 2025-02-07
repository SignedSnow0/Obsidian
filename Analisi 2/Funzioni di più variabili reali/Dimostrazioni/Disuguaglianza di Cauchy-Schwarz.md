---
subject: analisi 2
type: dimostrazione
---
Siano $x,y\in\mathbb{R}^n$, allora
$$
|x\cdot y|\le||x||||y||
$$

# Dimostrazione
Sia per $t\in\mathbb{R}$
$$
P(t)=(x+ty)\cdot(x+ty)
$$
Grazie alle proprietà dello spazio vettoriale $\mathbb{R}^n$ e la definizione di [[Analisi 2/Funzioni di più variabili reali/Norma|norma]] si ottiene
$$
P(t)=x\cdot x+2t(x\cdot y)+t^2(y\cdot y)
$$
Perciò $P(t)\ge0\forall t\in\mathbb{R}$, quindi
$$
(x\cdot y)^2-(x\cdot x)(y\cdot y)\le0
$$
$$
(x\cdot y)^2\le(x\cdot x)(y\cdot y)\quad\square
$$

##### Correlati:
* [[Prodotto scalare]]