---
subject: fondamenti di telecomunicazioni
---
Sia $x$ un segnale complesso e la sua trasformata $\mathcal{F}[x]=X$, allora si hanno le seguenti proprietà
> [!remark] Coniugazione
> $$
> \mathcal{F}[x^*(t)]=X^*(-\omega)
> $$

> [!remark] Traslazione temporale
> $$
> \mathcal{F}[x(t-t_0)]=X(\omega)\e^{-j\omega t_0}
> $$

> [!remark] Derivata
> $$
> \mathcal{F}[\dot{x}]=j\omega X
> $$

> [!remark] Integrale
> $$
> \mathcal{F}\left[\int_{-\infty}^tx(\zeta)d\zeta\right]=\frac{X}{j\omega}\quad\text{se } X(0)=\int_{-\infty}^{+\infty}dtx=0
> $$

> [!remark] Convoluzione
> $$
> \mathcal{F}[x*y]=XY
> $$
> $$
> [x*y](t)=\int_{-\infty}^{+\infty}d\tau x(\tau)y(t-\tau)
> $$