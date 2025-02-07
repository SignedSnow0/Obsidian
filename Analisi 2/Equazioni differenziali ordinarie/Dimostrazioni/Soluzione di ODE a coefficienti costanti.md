---
subject: analisi 2
type: dimostrazione
---
Sia un equazione differenziale del tipo
$$
x^{(m)}(t)=a_0x(t)+\dots+a_{m-1}x^{(m-1)}(t)
$$
cioè a coefficienti costanti, sia $\lambda_0\in\mathbb{R}:P(\lambda_0)=0$ dove $P$ è il [[Polinomio caratteristico di un ODE lineare a coefficienti costanti|polinomio caratteristico]] dell'equazione, allora 
$$
x(t)=e^{\lambda_0t}
$$
è una [[Soluzione massimale|soluzione massimale]] con dominio $\mathbb{R}$
# Dimostrazione
Si ha $\forall t\in\mathbb{R}$
$$
x'(t)=\lambda_0e^{\lambda_0t},\dots,x^{(m-1)}(t)=\lambda_0^{m-1}e^{\lambda_0t}
$$
allora
$$
x^{(m)}(t)-a_0x(t)-\dots-a_{m-1}x^{(m-1)}(t)=P(\lambda_0)e^{\lambda_0t}=0\quad\square
$$