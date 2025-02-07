---
subject: analisi 2
type: dimostrazione
---
Sia $A\subseteq\mathbb{R}^n$ aperto [[Stellato|stellato]] per qualche punto $x^0,F\in\mathcal{C}^1(A;\mathbb{R}^n)$ [[Campo vettoriale chiuso|chiuso]], allora $F$ è [[Campo vettoriale esatto|esatto]].
# Dimostrazione
Per $x\in A$ poniamo 
$$
\alpha^x:[0,1]\to\mathbb{R}^n,\quad\alpha^x(t)=x^0+t(x-x^0)
$$
$\alpha^x$ rappresenta il [[Segmento|segmento]] di estremi $x^0,x$ con sostegno in $A$, sia
$$
U:A\to\mathbb{R},\quad U(x)=\int F\cdot d\alpha^x=\sum_{j=1}^{n}(x_j-x^0_j)\int_0^1F_j(x^0+t(x-x^0))dt
$$
sia $\displaystyle V(t)=\int_0^1F_j(x^0-t(x-x^0))dt$ e scambiando la derivata con l'integrale poniamo 
$$
W(t)=F_j(x^0+t(x-x^0))
$$
allora 
$$
\frac{\partial W_t}{\partial x_i}(x)=t\frac{\partial F_j}{\partial x_i}(x^0+t(x-x^0))
$$
quindi
$$
\frac{\partial V_j}{\partial x_i}(x)=\int_0^1\frac{\partial W_t}{\partial x_i}(x)dt=\int_0^1t\frac{\partial F_j}{\partial x_i}(x^0+t(x-x^0))dt
$$
usando che $F$ è chiuso poniamo
$$
r:[0,1]\to\mathbb{R},\quad r(t)=F_i(x^0+t(x-x^0))
$$
allora $\displaystyle r'(t)=\sum_{j=1}^{n}\frac{\partial F_i}{\partial x_j}(x^0+t(x-x^0))(x_j-x^0_j)$, allora per la formula di integrazione per parti
$$
\frac{\partial U}{\partial x_i}(x)=\int_0^1tr'(t)dt+\int_0^1r(t)dt=[tr(t)]_0^1-\int_0^1r(t)dt+\int_0^1r(t)dt=r(1)=F_i(x)\quad\square
$$

##### Correlati: