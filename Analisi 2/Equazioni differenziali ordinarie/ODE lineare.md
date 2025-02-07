---
subject: analisi 2
type: definizione
---
Un [[Equazione differenziale|equazione differenziale]] lineare è della forma
$$
x^{(m)}(t)=a_0(t)x(t)+\dots+a_{m-1}(t)x^{(m-1)}(t)+b(t)
$$
con $a_0,\dots,a_{m-1},b:I\to\mathbb{R},I\subseteq{R}$ aperto e continue. 
Notiamo che
$$
f:\Omega\to\mathbb{R},\quad f(t,X_0,\dots,X_{m-1})=a_0(t)x(t)+\dots+a_{m-1}(t)x^{(m-1)}(t)+b(t)
$$
$$
t\in I,X_0,\dots,X_{m-1}\in\mathbb{R}
$$
perciò un equazione di questo tipo soddisfa le ipotesi del [[Teorema di Picard|teorema di Picard]] perchè
1. $f\in\mathcal{C}$
2. $\forall j\in\{0,\dots,m-1\}$ si ha $\frac{\partial f}{\partial X_j}(t,X_1,\dots,X_{m-1})=a_j(t)\in\mathcal{C}(I)$

allora comunque si prendano $t_0\in I,y_0,\dots,y_{m-1}\in\mathbb{R}$, il [[Problema di Cauchy|problema di Cauchy]]
$$
\begin{cases}x^{(m)}(t)=a_0(t)x(t)+\dots+a_{m-1}(t)x^{(m-1)}(t)+b(t)\\x(t_0)=y_0\\\vdots\\x^{(m-1)}(t_0)=y_{m-1}\end{cases}
$$
ha un'unica [[Soluzione massimale|soluzione massimale]] e il suo dominio è $I$.