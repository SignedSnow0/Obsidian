---
subject: analisi 1
type: dimostrazione
---
Sia $f$ n-volte derivabile in $x_0$, se esiste un polinomio $P_n$ di grado n tale che $f(x)=P_n(x)+o((x-x_0)^n)$, allora
$$
Tf_{n,x_0}(x)=P_n(x)
$$
# Dimostrazione
Visto che entrambe le funzioni sono polinomi possiamo scrivere
$$
P_n(x)-Tf_{n,x_0}(x)=\sum_{k=0}^{n}(a_k-b_k)(x-x_0)^k
$$
Inoltre sono entrambi o-piccoli di $(x-x_0)^n$ , quindi
$$
0=\lim_{x\to x_0}\frac{\displaystyle\sum_{k=0}^{n}(a_k-b_k)(x-x_0)^k}{(x-x_0)^j}\quad\forall j\in\{0,\dots,n\}
$$
Perciò in ogni grado la differenza tra i due polinomi è zero, quindi coincidono $\square$