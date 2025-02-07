---
subject: fondamenti di telecomunicazioni
---
> [!remark] Parità
> $$
> \int_\mathbb{R}dtx\delta(t-t_0)=\int_\mathbb{R}dtx\delta(t_0-t)
> $$

> [!remark] Convoluzione
> $$
> x(t)=\int_\mathbb{R}d\tau x(\tau)\delta(t-\tau)=(x*\delta)(t)
> $$

> [!remark] Cambio di argomento
> $$
> \delta(\alpha t)=\frac{\delta}{|\alpha|}
> $$

> [!remark] Trasformata di Fourier
> $$
> \int_\mathbb{R}dt\delta e^{-j\omega t}=1
> $$

> [!remark] Gradino unitario
> Definiamo la funzione gradino unitario come
> $$
> U(t)=\begin{cases}1&t>0\\0&t<0\end{cases}
> $$
> allora
> $$
> \frac{dU(t-t_0)}{dt}=\delta(t-t_0)
> $$
> $$
> U(t-t_0)=\int_{-\infty}^{t-t_0}d\tau\delta(\tau)
> $$