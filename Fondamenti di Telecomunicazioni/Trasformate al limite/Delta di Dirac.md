---
subject: fondamenti di telecomunicazioni
---
Il delta di Dirac è una distribuzione di funzioni con le seguenti proprietà:
> [!remark] Proprietà del delta di Dirac
> $$
> \delta_{t_0}=\begin{cases}0&t\ne t_0\\1&t=t_0\end{cases}\quad\int_\mathbb{R}dt\delta_{t_0}=1
> $$
In maniera formale per ottenere questa distribuzione prendiamo una serie di funzioni $f_\Delta$ dove 
$$
f_\Delta=\begin{cases}\frac{1}{\Delta}&t\in[0,\Delta]\\0&t\notin[0,\Delta]\end{cases}
$$
in questo caso la funzione è un impulso rettangolare di durata $\Delta$ e ampiezza $\frac{1}{\Delta}$: $U(t,\Delta)$.
Allora il delta di Dirac è ottenuto nel limite dove $\Delta\to0$
> [!definition] Delta di Dirac
> $$
> \delta=\lim_{\Delta\to0}f_\Delta
> $$

> [!remark]
> Dato un segnale $x$ si ha che
> $$
> \langle x,\delta_{t_0}\rangle=x(t_0)
> $$
> `\begin{proof}`
> Dalla definizione di [[Rappresentazione ortonormale di segnali|prodotto interno]] e delta di Dirac si ha
> $$
> \langle x,\delta_{t_0}\rangle=\lim_{\Delta\to0}\int_\mathbb{R}dtxf_\Delta=x(t_0)
> $$
> `\end{proof}`