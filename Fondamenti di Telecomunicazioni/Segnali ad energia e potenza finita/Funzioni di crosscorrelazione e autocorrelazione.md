 > [!definition] Crosscorrelazione
> Dati due segnali $x,y$ si definisce crosscorrelazione il prodotto interno del coniugato di un segnale per il la versione anticipata dell'altro
> $$
> \dot\varphi_{x,y}(\tau)=\langle x,y_{\tau}\rangle^\dagger=\int_{\mathbb{R}}dtx^\dagger(t)y(t+\tau)
> $$

> [!remark] Anticommutatività
> $$
> \dot\varphi_{x,y}(\tau)=\dot\varphi^\dagger_{y,x}(-\tau)
> $$

> [!remark] Relazione con l'energia
> $$
> |\dot\varphi_{x,y}|^2\le\dot\varphi_x(0)=E_xE_y
> $$

> [!remark] Crosscorrelazione come convoluzione
> $$
> \dot\varphi_{x,y}(\tau)=x^\dagger(-\tau)*y(\tau)
> $$
---
> [!definition] Autocorrelazione
> La funzione di autocorrelazione è un caso particolare di crosscorrelazione dove il segnale è lo stesso
> $$
> \dot\varphi_{x}(\tau)=\langle x,x_{\tau}\rangle=\int_{\mathbb{R}}dtx^*(t)x(t+\tau)
> $$

> [!remark] Simmetria Hermitiana
> $$
> \dot\varphi_x(\tau)=\dot\varphi_x^\dagger(-\tau)
> $$

> [!remark] Relazione con l'energia
> $$
> |\dot\varphi_x|\le\varphi_x(0)=E_x
> $$

> [!remark] Autocorrelazione come convoluzione
> $$
> \dot\varphi_x(\tau)=x^\dagger(-\tau)*y(\tau)
> $$