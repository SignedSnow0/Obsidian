---
subject: fondamenti di telecomunicazioni
---
Sia $x$ un segnale [[Moto periodico|periodico]], quindi $x(t)=x(t+T)$ e la pulsazione è $\omega_0=\frac{2\pi}{T}$, allora $x$ è rappresentabile con la formula
> [!definition] Serie di Fourier
> $$
> x=\sum_{n=-\infty}^{+\infty}c_n\e^{jn\omega_0t}
> $$

dove ogni coefficiente $c_n$ è dato dal seguente integrale
> [!definition] Analisi di Fourier
> $$
> c_n=\frac{1}{T}\int_{-\frac{T}{2}}^{+\frac{T}{2}}dtx\e^{-jn\omega_0t}
> $$
