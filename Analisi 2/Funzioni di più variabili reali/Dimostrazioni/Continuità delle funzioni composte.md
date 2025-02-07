---
subject: analisi 2
type: dimostrazione
---
Sia $A\subseteq\mathbb{R}^n,B\subseteq\mathbb{R}^m,f:A\to\mathbb{R}^m:f(A)\subseteq B,g:B\to\mathbb{R}^l$, allora
1. se $x^0:f\in\mathcal{C}(x^0),g\in\mathcal{C}(f(x^0))\implies g\circ f\in\mathcal{C}(x^0)$
2. se $f,g\in\mathcal{C}\implies g\circ f\in\mathcal{C}$
# Dimostrazione
Sia $\epsilon\in\mathbb{R}^+$, poichè $g\in\mathcal{f(x^0)}$
$$
\exists\delta_1(\epsilon)\in\mathbb{R}^+:y\in B(f(x^0),\delta_1(\epsilon))\cap B\implies||g(y)-g(f(x^0))||_l<\epsilon
$$
inoltre poichè $f\in\mathcal{C}(x^0)$
$$
\exists\delta(\epsilon)\in\mathbb{R}^+:x\in B(x^0,\delta(\epsilon))\cap A\implies||f(x)-f(x^0)||_m<\delta_1(\epsilon)
$$
cioè $f(x)\in B(f(x^0),\delta_1(\epsilon))\cap B$, allora
$$
x\in B(x^0,\delta(\epsilon))\cap A\implies||g(f(x))-g(f(x^0))||_l<\epsilon\quad\square
$$

##### Correlati:
* [[Funzione continua]]