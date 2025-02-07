---
subject: analisi 2
type: definizione
---
Un [[Equazione differenziale|equazione differenziale]] a variabili separabili è un equazione della forma
$$
x'(t)=h(t)g(x(t))
$$
con $h:I_1\to\mathbb{R}\in\mathcal{C},g:I_2\to\mathbb{R}\in\mathcal{C}^1,I_1,I_2\subseteq\mathbb{R}$.
Ponendo $f:I_1\times I_2\to\mathbb{R},f(t,x)=h(t)g(x)$ abbiamo che $f\in\mathcal{C},$
$$
\forall(t,x)\in I_2\times I_2\quad\frac{\partial f}{\partial x}(t,x)=h(t)g'(x)
$$
sappiamo quindi che equazioni di questa forma rispettano le ipotesi del [[Teorema di Picard|teorema di Picard]].
Consideriamo ora il [[Problema di Cauchy|problema di Cauchy]]
$$
\begin{cases}x'(t)=h(t)g(x(t))\\ x(t_0)=x^0\end{cases}
$$
con $t_0\in I_1,x^0\in I_2$ allora esso ammette un unica [[Soluzione massimale|soluzione massimale]] con dominio in $I_2$.
Notiamo che se $x$ è [[Soluzione massimale|soluzione massimale]], allora $g(x(t))\ne 0\quad\forall t\in I\subseteq I_1$ , poniamo
$$
\frac{x'(t)}{g(x(t))}=h(t)\quad\forall t\in I
$$
$$
\int_{t^0}^{t}\frac{x'(s)}{g(x(s))}ds=\int_{t^0}^{t}h(s)ds
$$
Riguardo all'immagine di $x=J$ sappiamo che è sottointervallo di $I_2$ per [[Analisi 2/Funzioni di più variabili reali/Dimostrazioni/Teorema di Bolzano|teorema di Bolzano]] e visto che $g(x(t))\ne 0$ allora anche $g(y)\ne 0\quad\forall y\in J$, allora
$$
\int_{t^0}^{t}\frac{x'(s)}{g(x(s))}ds=G(x(t))-G(x(t^0))=G(x(t))-G(x^0)
$$
$$
G(x(t))=G(x^0)+\int_{t^0}^{t}h(s)ds
$$
$$
G'(y)=\frac{1}{g(y)}\ne0\quad\forall y\in J
$$
sempre per il [[Analisi 2/Funzioni di più variabili reali/Dimostrazioni/Teorema di Bolzano|teorema di Bolzano]] $G'(y)>0$ oppure $G'(y)<0$ per ogni $y\in J$, in ogni caso possiamo dire che $G$ è strettamente monotona e quindi iniettiva, perciò 
$$
x(t)=G^{-1}(G(x^0))+\int_{t_0}^{t}h(s)ds
$$