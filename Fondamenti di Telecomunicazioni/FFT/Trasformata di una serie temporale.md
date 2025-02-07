---
subject: fondamenti di telecomunicazioni
---
> [!definition] Trasformata di una serie temporale
> Data una [[Serie temporale|serie temporale]] $\{x_n\}$, la sua [[Trasformata di Fourier|trasformata]] è
> $$
> X_s=\sum_{n=-\infty}^{+\infty}x_n\e^{-jn\omega T}
> $$
> e ogni elemento della serie equivale all'[[Trasformata di Fourier|antitrasformata]]
> $$
> x_n=\frac{T}{2\pi}\int_{-\frac{\pi}{T}}^{\frac{\pi}{T}}d\omega X_s\e^{jn\omega T}
> $$
> `\begin{proof}`
> Notiamo che la trasformata stessa è una funzione periodica nelle frequenze di periodo $\omega_p=\frac{2\pi}{T}$, possiamo allora rappresentarla come [[Forma esponenziale di segnali complessi|serie di Fourier]] ricordando che è periodica nelle pulsazioni
> $$
> X_s=\sum_{n=-\infty}^{+\infty}c_n\e^{jn\omega t}=\sum_{n=-\infty}^{+\infty}c_n\e^{jn\omega\frac{2\pi}{\omega_p}}=\sum_{n=-\infty}^{+\infty}c_n\e^{jn\omega T}
> $$
> allora gli elementi $c_n$ saranno
> $$
> c_n=\frac{1}{\omega_p}\int_{-\frac{\omega_p}{2}}^{\frac{\omega_p}{2}}d\omega X_s\e^{-jn\omega T}=\frac{T}{2\pi}\int_{-\frac{\omega_p}{2}}^{\frac{\omega_p}{2}}d\omega X_s\e^{-jn\omega T}
> $$
> allora dichiarando $x_n=c_{-n}$ si ottiene la conclusione
> `\end{proof}`