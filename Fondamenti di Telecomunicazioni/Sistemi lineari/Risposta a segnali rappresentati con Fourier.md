---
subject: fondamenti di telecomunicazioni
---
Se il segnale è rappresentabile con una [[Forma esponenziale di segnali complessi|serie di Fourier]] allora
$$
Y=XH
$$
espandendo il segnale in ingresso $x$ si ha
$$
y=\sum_{n=-\infty}^{+\infty}c_nH(n\omega_0)\e^{jn\omega_0t}
$$
che per un segnale reale diventa
$$
y=A_0H(0)+\sum_{n=1}^{+\infty}A_nT(n\omega_0)\cos[n\omega_0t-\phi_n-\beta(n\omega_0)]
$$
oppure in forma [[Trasformata di Fourier|continua]] si ha
$$
y=\int_{0}^{+\infty}d\omega VT\cos[\omega t-\phi-\beta]
$$
dove 
$$
T=|H|
$$
$$
\beta=-\angle H
$$