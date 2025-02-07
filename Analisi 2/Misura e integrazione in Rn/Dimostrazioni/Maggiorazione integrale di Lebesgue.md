---
subject: analisi 2
type: dimostrazione
---
Sia $A\in\mathcal{M}_n,f:A\to\mathbb{R}$ [[Funzione sommabile|sommabile]], allora
$$
\left|\int_Af(x)dx\right|\le\int_A|f(x)|dx
$$
# Dimostrazione
$$
\left|\int_Af(x)dx\right|=\left|\int_Af_+(x)dx-\int_Af_-(x)dx\right|\le\int_Af_+(x)dx+\int_Af_-(x)dx=\int_A|f(x)|dx\quad\square
$$