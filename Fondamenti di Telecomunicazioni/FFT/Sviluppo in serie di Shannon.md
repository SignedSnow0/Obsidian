---
subject: fondamenti di telecomunicazioni
---
Lo sviluppo in serie di Shannon è lo [[Forma esponenziale di segnali complessi|sviluppo]] di $x$ a partire dai valori campionati $x_n$ sotto le condizioni del [[Teorema di Shannon|teorema di Shannon]]
> [!definition] Serie di Shannon
> $$
> x=\sum_{n=-\infty}^{+\infty}x_n\sinc\left(\frac{t-nT}{T}\right)
> $$
> `\begin{proof}`
> Esprimiamo il segnale come la sua [[Trasformata di Fourier|trasformata]], ricordiamo il [[Serie temporale|lemma]] e prendiamo come massimo la [[Teorema di Shannon|frequenza di Nyquist]], allora
> $$
> X=\begin{cases}TX_s&|\omega|<\frac{\omega_0}{2}\\0\end{cases}
> $$
> facciamo ora l'[[Trasformata di Fourier|antitrasformata]]
> $$
> x=\frac{1}{2\pi}\int_\mathbb{R}d\omega X\e^{j\omega t}=\frac{T}{2\pi}\int_{-\frac{\pi}{T}}^{\frac{\pi}{T}}d\omega X_s\e^{j\omega t}
> $$
> sostituendo $X_s$ con la sua [[Trasformata di una serie temporale|trasformata]]
> $$
> x=\frac{T}{2\pi}\sum_{n=-\infty}^{+\infty}x_n\int_{-\frac{\pi}{T}}^{\frac{\pi}{T}}d\omega\e^{j\omega t}\e^{-jn\omega T}
> $$
> risolviamo allora un singolo termine integrale
> $$
> \frac{T}{2\pi}\int_{-\frac{\pi}{T}}^{\frac{\pi}{T}}d\omega\e^{j\omega t}\e^{-jn\omega T}=\frac{T}{2\pi}\eval{\frac{\e^{j\omega(t-nT)}}{j(t-nT)}}{-\frac{\pi}{T}}{\frac{\pi}{T}}=\frac{T}{2\pi}\frac{2\e^{\frac{\pi}{T}(t-nT)}}{j(t-nT)}
> $$
> passando dalla rappresentazione polare alla rappresentazione trigonometrica si ha
> $$
> \frac{\sin\left(\pi\frac{t-nT}{T}\right)}{\pi\frac{t-nT}{T}}=\sinc\left(\frac{t-nT}{T}\right)
> $$
> mettendo la soluzione nella seria si ha
> $$
> x=\sum_{n=-\infty}^{+\infty}x_n\sinc\left(\frac{t-nT}{T}\right)
> $$
> `\end{proof}`

I termini della serie $\sinc$ hanno banda $\left[0,\frac{\omega_0}{2}\right]$ e sono fra di loro [[Ortogonale di un vettore|ortogonali]].