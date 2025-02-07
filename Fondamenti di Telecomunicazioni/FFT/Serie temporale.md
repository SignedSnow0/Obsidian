---
subject: fondamenti di telecomunicazioni
---
Se la funzione è discreta nel tempo viene chiamata serie temporale, di solito sono il prodotto del campionamento di una funzione continua ad intervalli costanti.
> [!definition] Serie per campionamento
> Dato un valore continuo nel tempo si ottiene una serie per campionamento se i valori della serie sono ottenuti dal segnale ad intervalli costanti, cioè
> $$
> x_n=x(nT)
> $$

Se la serie è ottenuta per campionamento vale la seguente relazione
> [!lemma] Trasformata del segnale e dei campioni
> $$
> X_s=\frac{1}{T}\sum_{k=-\infty}^{+\infty}X(\omega+k\omega_0)
> $$
> `\begin{proof}`
> Esprimiamo gli elementi $x_n$ come [[Trasformata di Fourier|antitrasformate]]
> $$
> x_n=\frac{T}{2\pi}\int_{-\frac{\pi}{T}}^{\frac{\pi}{T}}d\omega X_s\e^{jn\omega T}
> $$
> facciamo lo stesso con il segnale calcolato in $nT$
> $$
> x(nT)=\frac{1}{2\pi}\int_\mathbb{R}d\omega X\e^{j\omega nT}
> $$
> dividiamo ora l'integrale su $\mathbb{R}$ in intervalli contigui di ampiezza $\frac{2\pi}{T}$
> $$
> x(nT)=\frac{1}{2\pi}\sum_{k=-\infty}^{+\infty}\int_{-\frac{\pi}{T}+k\omega_0}^{\frac{\pi}{T}+k\omega_0}d\omega X\e^{j\omega nT}
> $$
> facciamo il cambio di variabile $\eta=\omega-k\omega_0$
> $$
> x(nT)=\frac{1}{2\pi}\sum_{n=-\infty}^{+\infty}\int_{-\frac{\pi}{T}}^{\frac{\pi}{T}}d\eta X(\eta+k\omega_0)\e^{j(\eta+k\omega_0)nT}=
> $$
> $$
> =\frac{1}{2\pi}\sum_{n=-\infty}^{+\infty}\int_{-\frac{\pi}{T}}^{\frac{\pi}{T}}d\eta X(\eta+k\omega_0)\e^{j\eta nT}\e^{jk\omega_0 nT}
> $$
> ricordando che ogni multiplo di $k\omega_0$ è una pulsazione completa si ha
> $$
> x(nT)=\frac{1}{2\pi}\sum_{k=-\infty}^{+\infty}\int_{-\frac{\pi}{T}}^{\frac{\pi}{T}}d\eta X(\eta+k\omega_0)\e^{j\eta nT}
> $$
> mettendo assieme abbiamo
> $$
> x(nT)=\frac{1}{2\pi}\sum_{k=-\infty}^{+\infty}\int_{-\frac{\pi}{T}}^{\frac{\pi}{T}}d\omega X(\omega+k\omega_0)\e^{j\omega nT}=\frac{T}{2\pi}\int_{-\frac{\pi}{T}}^{\frac{\pi}{T}}d\omega X_s\e^{jn\omega T}=x_n
> $$
> facendo la [[Trasformata di Fourier|trasformata]] otteniamo la dimostrazione
> `\end{proof}`