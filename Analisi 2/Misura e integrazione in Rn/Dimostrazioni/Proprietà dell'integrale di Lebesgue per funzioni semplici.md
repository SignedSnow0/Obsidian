---
subject: analisi 2
type: dimostrazione
---
Sia $A\in\mathcal{M}_n,f,g:A\to\mathbb{R}$  [[Funzione semplice|semplice]] non negative, allora:
1. $\displaystyle\int_Af(x)dx\in[0,+\infty]$
2. se $f(x)\le g(x)\quad\forall x\in A$, allora $\displaystyle\int_Af(x)dx\le\int_Ag(x)dx$
3. $\displaystyle\int_A(f+g)(x)dx=\int_Af(x)dx+\int_Ag(x)dx$
4. se $\alpha\in[0,+\infty),\alpha f$ è [[Funzione semplice|semplice]] non negativa e
$$
\int_A\alpha f(x)dx=\alpha\int_Af(x)dx
$$
5. se $B=B_1\cup\dots\cup B_p$ misurabili e disgiunti
$$
\int_Af(x)dx=\sum_{i=1}^{p}\int_{B_i}f(x)dx
$$
con $\displaystyle\int_{B_i}f(x)dx=\int_{B_i}f_{|B_i}(x)dx$
# Dimostrazione
Il punto 1 segue dalla definizione di [[Integrale di Lebesgue per funzione semplice|integrale]].
Secondo il [[Algebra delle funzioni semplici#Lemma|lemma]] abbiamo che $\exists\alpha_i,\beta_i:\alpha_i\le\beta_i\quad\forall i\in\{1,\dots,m\}$ perciò
$$
\int_Af(x)dx=\sum_{i=1}^{m}\alpha_iL_n(A_i)\le\sum_{i=1}^{m}\beta_iL_n(A_i)=\int_Ag(x)dx
$$
provando il secondo punto.
Per [[Algebra delle funzioni semplici|algebra delle funzioni semplici]]
$$
\int_A(f+g)(x)dx=\sum_{k=1}^{m}(\alpha_k+\beta_k)L_n(A_k)=\sum_{k=1}^{m}\alpha_kL_n(A_k)+\sum_{k=1}^{m}\beta_kL_n(A_k)=\int_Af(x)dx+\int_Ag(x)dx
$$
Per $\alpha f(x)=\alpha\alpha_i$
$$
\int_A\alpha f(x)dx=\sum_{k=1}^{m}\alpha\alpha_kL_n(A_k)=\alpha\sum_{k=1}^{m}\alpha_kL_n(A_k)=\alpha\int_Af(x)dx
$$
Sia $p=2$, allora per $j\in\{1,2\}$ si ha
$$
B_j=(B_j\cap A_1)\cup\dots\cup(B_j\cap A_m)
$$
le intersezioni sono disgiunte e misurabili, quindi
$$
\int_{B_1}f(x)dx+\int_{B_2}f(x)dx=\sum_{k=1}^{m}\alpha_kL_n(A_k\cap B_1)+\sum_{k=1}^{m}\alpha_kL_n(A_k\cap B_2)=\sum_{k=1}^{m}\alpha_k[L_n(A_k\cap B_1)+L_n(A_k\cap B_2)]=
$$
$$
\sum_{k=1}^{m}\alpha_kL_n(A_k)=\int_Af(x)dx
$$
osservando che $(A_i\cap B_1)\cup(A_i\cap B_2)=A_i$ si conclude la dimostrazione.$\quad\square$