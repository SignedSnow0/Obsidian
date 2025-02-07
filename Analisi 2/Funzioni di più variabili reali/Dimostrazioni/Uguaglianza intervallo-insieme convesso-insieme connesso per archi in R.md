---
subject: analisi 2
type: dimostrazione
---
Sia $A\subseteq\mathbb{R}$, allora
$$
A\text{ è un intervallo}\iff A\text{ è convesso}\iff A\text{ è connesso per archi}
$$
# Dimostrazione
Sia $A$ intervallo, $x,y\in A, t\in[0,1]$, se $x\le y$
$$
x\le x+t(y-x)\le x+(y-x)=y
$$
se invece $y\ge y$
$$
y=x+(y-x)\le x+t(y-x)\le x
$$
visto che $A$ è intervallo $x+t(y-x)\in A\quad\forall t\in[0,1]$ perciò $A$ è convesso.

Inoltre tutti i convessi sono connessi per archi.

Sia ora $A$ connesso per archi, $x,y\in A,x\le y$, poichè $A$ è connesso per archi
$$
\exists a,b\in\mathbb{R},a\le b,\phi:[a,b]\to\mathbb{R}\in\mathcal{C}:\phi(a)=x,\phi(b)=y
$$
allora per il [[Analisi 1/Continuità/Dimostrazioni/Teorema di Bolzano|Teorema di Bolzano]]
$$
z\in\phi([a,b])\subseteq A\quad\square
$$

##### Correlati:
* [[Intervallo]]
* [[Insieme convesso]]
* [[Insieme connesso per archi]]