---
subject: analisi 2
type: definizione
---
Sia
$$
\phi_+:\mathbb{R}\to\mathbb{R},\quad\phi_+(x)=\max\{x,0\}
$$
$$
\phi_-:\mathbb{R}\to\mathbb{R},\quad\phi_-(x)=\min\{-x,0\}
$$
abbiamo allora le seguenti proprietà
1. $\phi_+,\phi_-\in\mathcal{C}$
2. $\forall x\in\mathbb{R}\quad x=\phi_+(x)-\phi_-(x)$
3. $\forall x\in\mathbb{R}\quad|x|=\phi_+(x)+\phi_-(x)$
4. $\phi_{\pm}$ sono a valori non negativi

Inoltre per ogni insieme abbiamo $f_{\pm}=\phi_{\pm}\circ f$
1. $\forall x\in\mathbb{R}\quad f(x)=f_+(x)-f_-(x)$
2. $\forall x\in\mathbb{R}\quad|f(x)|=f_+(x)+f_-(x)$
3. $f_{\pm}$ sono [[Funzione misurabile|misurabili]] a valori non negativi (per [[Algebra delle funzioni misurabili|proprietà funzioni misurabili]])

Diremo che $f$ è sommabile in $A\in\mathcal{M}_n$ se 
$$
\int_A|f(x)|dx<+\infty
$$
dove l'integrale è [[Integrale di Lebesgue per funzione misurabile|definito]] su una [[Funzione misurabile|funzione misurabile]].