---
subject: analisi 2
type: dimostrazione
---
Sia $A\subseteq\mathbb{R}^n$ connesso per archi, $f:A\to\mathbb{R}^m\in\mathcal{C}$, allora:
1. $f(A)$ è connesso per archi in $\mathbb{R}^m$
2. se $m=1\implies f(A)$ è un intervallo
# Dimostrazione
Sia $v,w\in f(A), x,y\in A:f(x)=v,f(y)=w$, poichè $A$ è connesso per archi
$$
\exists a,b\in\mathbb{R},a\le b,\quad \phi:[a,b]\to\mathbb{R}^n\in\mathcal{C}:\phi(a)=x,\phi(b)=y
$$
Sia ora
$$
\psi:[a,b]\to\mathbb{R}^m,\quad\psi(t)=f(\phi(t)),\quad t\in[a,b]
$$
allora per [[Continuità delle funzioni composte]]: $\psi\in\mathcal{C},\quad \psi(a)=f(\phi(a))=v,\psi(b)=f(\phi(b))=w$, quindi $f(A)$ è connesso per archi $\quad\square$

##### Correlati:
* [[Insieme connesso per archi]]
* [[Funzione continua]]
* [[Intervallo]]