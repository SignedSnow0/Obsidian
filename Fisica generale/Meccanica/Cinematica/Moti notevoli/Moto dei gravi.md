---
subject: fisica generale
type: definizione
---
Il moto dei gravi ha [[Accelerazione scalare|accelerazione]] costante 
$$
\vec{a}=-g\hat{j}=\vec{g}
$$
dove $g$ rappresenta l'[[Accelerazione scalare|accelerazione]] gravitazionale  ($9.81\space m/s^2$), risolvendo i [[Problema di Cauchy|problemi di Cauchy]] si ha
$$
\vec{v}(t)=\vec{v}_0+\int_{t_0}^t\vec{g}dt=\vec{v}_0+\vec{g}\int_{t_0}^tdt=\vec{v}_0+g(t-t_0)
$$
$$
\vec{r}(t)=\vec{r}_0+\int_{t_0}^t\vec{v}(s)ds=\vec{r}_0+\int_{t_0}^t(\vec{v}_0+\vec{g}(s-s_0))ds=\vec{r}_0+\vec{v}_0(t-t_0)+\frac12\vec{g}(t-t_0)^2
$$
Osserviamo che la [[Traiettoria|traiettoria]] è [[Moto rettilineo uniformemente accelerato|rettilinea]] lungo $\hat{j}$ se $\vec{v}_0=0$ o se $\vec{v}_0$ ha la stessa direzione di $\vec{g}$, mentre negli altri casi la [[Traiettoria|traiettoria]] è una parabola.
Ponendo $t_0=0,\vec{r}_0=\vec{0}$ e $\alpha$ come l'angolo tra $\vec{v}_0$ e $\hat{i}$, le equazioni sono del tipo
$$
\vec{v}(t)=(v_0\cos\alpha)\hat{i}+(v_0\sin\alpha-gt)\hat{j}
$$
$$
\vec{r}(t)=(v_0\cos(\alpha)t)\hat{i}+\left((v_0\sin(\alpha)t-\frac12gt^2\right)\hat{j}
$$
![[Moto dei gravi.excalidraw]]