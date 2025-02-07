---
subject: analisi 2 
type: dimostrazione
---
Sia $A\subseteq\mathbb{R}^n,x^0\in D(A),f:A\to\mathbb{R}^m,f(x)=(f_1(x),\dots,f_m(x)),l\in\mathbb{R}^m,l=(l_1,\dots,l_m)$, allora
$$
\lim_{x\to x^0}f(x)=l\iff\forall i\in\{1,\dots,m\}\lim_{x\to x^0}f_i(x)=l_i
$$
# Dimostrazione
* Sia $\displaystyle\lim_{x\to x^0}f(x)=l$, allora 
$$
\exists\delta(\epsilon)\in\mathbb{R}^+:x\in B(x^0,\delta(\epsilon))\cap A,x\ne x^0\implies||f(x)-l||_m<\epsilon
$$
per la [[Analisi 2/Funzioni di più variabili reali/Dimostrazioni/Proprietà della norma#^9cd2bc|proprietà della norma euclidea]] abbiamo
$$
|f_i(x)-l_i|\le||f(x)-l||_m<\epsilon
$$
* Sia invece ora $\displaystyle\forall i\in\{1,\dots,m\}\lim_{x\to x^0}f_i(x)=l_i$, sia $\epsilon,\eta\in\mathbb{R}^+$, allora
$$
\forall i\in\{1,\dots,m\}\quad\exists\delta_i(\eta)>0:x\in B(x^0,\delta(\eta))\cap A,x\ne x^0\implies|f_i(x)-l_i|<\eta
$$
sia $\delta(\eta)=\min\{\delta_i(\eta)|1\le i\le m\}$, allora
$$
||f(x)-l||=\sqrt{\sum_{i=1}^{m}(f_i(x)-l_i)^2}<\sqrt{(m\eta^2)}=\sqrt{m}\eta$$
scegliendo $\eta=\frac{\epsilon}{\sqrt{m}}$
$$
||f(x)-l||<\epsilon\quad\square
$$

##### Correlati:
* [[Limite]]