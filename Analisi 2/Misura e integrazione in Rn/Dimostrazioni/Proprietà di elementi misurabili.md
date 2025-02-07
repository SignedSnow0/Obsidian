---
subject: analisi 2
type: dimostrazione
---
1. $\mathbb{R}^n\in\mathcal{M}_n$
2. se $a_k$ è una successione di elementi in $\mathcal{M}_n$, allora $\displaystyle\bigcap_{k\in\mathbb{N}}a_k\in\mathcal{M}_n$
3. se $A_1,\dots,A_m$ sono elementi di $\mathcal{M}_n$, allora $\displaystyle\bigcup_{k\in\{1,\dots,m\}}A_k\in\mathcal{M}_n$
4. se $A_1,\dots,A_m$ sono elementi di $\mathcal{M}_n$, allora $\displaystyle\bigcap_{k\in\{1,\dots,m\}}A_k\in\mathcal{M}_n$
5. se $A,B\in\mathcal{M}_n$, allora $B\setminus A\in\mathcal{M}_n$
6. se $A_1,\dots,A_m$ sono elementi di $\mathcal{M}_n$ a due a due disgiunti, allora
$$
L_n(\bigcup_{k\in\{1,\dots,m\}}A_k)=\sum_{k=1}^{m}L_n(A_k)
$$
7. se $A,B\in\mathcal{M}_n,A\subseteq B,L_n(B)<+\infty$ allora $L_n(A)<+\infty$ e
$$
L_n(B\setminus A)=L_n(B)-L_n(A)
$$
# Dimostrazione
Si ha che $\mathbb{R}^n=\emptyset^c$, per [[Teorema di Caratheodory|teorema di Caratheodory]] 1 è dimostrato.
Per il [[Proprietà di elementi misurabili#Lemma|lemma]]
$$
\bigcap_{k\in\mathbb{N}}a_k=(\bigcup_{k\in\mathbb{N}}a_k^c)^c
$$
perciò sempre per [[Teorema di Caratheodory|teorema di Caratheodory]] 2 è dimostrato.
Sia $A_k=\emptyset$, se $k>m$ allora per [[Teorema di Caratheodory|teorema di Caratheodory]] 3 è dimostrato.
Il punto 4 è analogo a 2 usando 3.
Si ha che $B\setminus A=B\cap A^c$, allora 5 è dimostrato con [[Teorema di Caratheodory|teorema di Caratheodory]].
Per 3 sappiamo che
$$
\bigcup_{k\in\{1,\dots,m\}}A_k\in\mathcal{M}_n
$$
inoltre ponendo $A_k=\emptyset,k>m$ e da [[Teorema di Caratheodory|teorema di Caratheodory]] si ha
$$
L_n(\bigcup_{k\in\{1,\dots,m\}}A_k)=L_n(\bigcup_{k\in\mathbb{N}}A_k)=\sum_{k=1}^{\infty}L_n(A_k)=\sum_{k=1}^{\infty}L_n(A_k)
$$
Si ha $B=A\cup(B\setminus A),A\cap(B\setminus A)=\emptyset$, perciò usando 6 si ha
$$
L_n(B)=L_n(A)+L_n(B\setminus A)\quad\square
$$

# Lemma
Sia $\{A_i|i\in\mathcal{I}\}$, un famiglia di sottoinsiemi di $\mathbb{R}^n$ con $\mathcal{I}$ un insieme di indici, allora
$$
\left(\bigcup_{i\in\mathcal{I}}A_i\right)^c=\bigcap_{i\in\mathcal{I}}A_i^c
$$
# Dimostrazione
Sia $x\in\mathbb{R}^n$, allora
$$
x\in\left(\bigcup_{i\in\mathcal{I}}A_i\right)^c\iff x\notin\bigcup_{i\in\mathcal{I}}A_i
$$
quindi
$$
x\in A_i^c\iff x\in\bigcap_{i\in\mathcal{I}}A_i^c
$$