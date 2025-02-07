---
subject: analisi 2
type: dimostrazione
---
Sia $A\in\mathcal{M}_n$, $f,g:A\to\mathbb{R}$ [[Funzione semplice|semplice]], allora
1. $f+g,fg$ sono [[Funzione semplice|semplici]]
2. se $g(x)\ne0$ allora $\frac fg$ è [[Funzione semplice|semplice]]
# Dimostrazione
Per il [[Algebra delle funzioni semplici#Lemma|lemma]] esistono $A_1,\dots,A_m$ sottoinsiemi partizione di $A$ e $\alpha_1,\dots,\alpha_m,\beta_1,\dots,\beta_m$ tali che se $x\in A_i\implies f(x)=\alpha_i,g(x)=\beta_i$, allora
$$
(f+g)(x)=f(x)+g(x)=\alpha_i+\beta_i\quad\square
$$

# Lemma
Sia $A\in\mathcal{M}_n,f,g:A\to\mathbb{R}$ [[Funzione semplice|semplice]], allora $\exists A_1,\dots, A_m$ partizione di $A$ e numeri reali $\alpha_1,\dots,\alpha_m,\beta_1,\dots,\beta_m$ tali che se 
$$
x\in A_i\implies f(x)=\alpha_i,g(x)=\beta_i
$$
## Dimostrazione
Sia $A=B_1\cup B_2,B_1,B_2\in\mathcal{M}_n,B_1\cap B_2=\emptyset,\exists\gamma_1,\gamma_2:$ se $x\in B_1,f(x)=\gamma_1,$ se $x\in B_2,f(x)=\gamma_2$
allo stesso modo supponiamo $A=C_1\cup C_2,C_1,C_2\in\mathcal{M}_n,C_1\cap C_2=\emptyset,\exists\delta_1,\delta_2:$ se $x\in C_1,f(x)=\delta_1,$ se $x\in C_2,f(x)=\delta_2$
poniamo 
$$
A_1=B_1\cap C_1,A_2=B_1\cap C_2,A_3=B_2\cap C_1,A_4=B_2\cap C_2
$$
allora $A_1,A_2,A_3,A_4\in\mathcal{M}_n$ e partizione di $A$, infine ponendo
$$
\alpha_1=\alpha_2=\gamma_1,\alpha_3=\alpha_4=\gamma_2
$$
$$
\beta_1=\beta_3=\delta_1,\beta_2=\beta_4=\delta_2
$$
si ha la conclusione. $\quad\square$
