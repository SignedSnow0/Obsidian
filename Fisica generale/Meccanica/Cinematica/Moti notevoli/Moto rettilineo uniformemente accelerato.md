---
subject: fisica generale
type: definizione
---
Il moto rettilineo uniformemente accelerato ha [[Accelerazione scalare|accelerazione]] costante, espressa dalla formula
$$
\vec{a}=\ddot{s}\hat{u}_t
$$
visto che il moto si muove su una retta l'[[Accelerazione vettoriale|accelerazione]] ha solo [[La componente|componente]] tangenziale in quanto il [[Cerchio osculatore|raggio di curvatura]] tende a $\infty$ e perciò $\vec{a}_n\to0$.
Inoltre, sempre per la restrizione geometrica, anche il [[Versore|versore]] $\hat{u}_t$ è costante.
Risolvendo i [[Problema di Cauchy|problemi di Cauchy]] si ha
$$
v(t)=v_0+\int_{t_0}^tadt=v_0+a\int_{t_0}^tdt=v_0+a(t-t_0)
$$
$$
s(t)=s_0+\int_{t_0}^t(v_0+as)ds=s_0+v_0(t-t_0)+\frac12a(t^2-t_0^2)
$$
scegliendo $v_0=v(t_0),s_0=s(t_0),t_0=0$ si ha
$$
v(t)=v_0+at
$$
$$
s(t)=s_0+v_0t+\frac12at^2
$$
la restrizione di tipo geometrico inoltre permette di poter definire facilmente il moto definendo un sistema di riferimento con un asse parallelo alla retta della [[Traiettoria|traiettoria]]
$$
\vec{a}=a_x\hat{i}
$$
$$
v_x=v_{0x}+a_xt
$$
$$
s(t)=x(t)=x_0+v_{0x}t+\frac12a_xt^2
$$
$$
\vec{r}(t)=x(t)\hat{i}
$$
![[Moto rettilineo.excalidraw]]
