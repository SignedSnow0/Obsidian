> [!theorem] Teorema di Parseval generalizzato
> Dati due segnali $x,y$ [[Trasformata di Fourier|trasformabili]] si ha
> $$
> \langle x,y\rangle=\frac{1}{2\pi}\langle X,Y\rangle
> $$
> cioè
> $$
> \int_{\mathbb{R}}dtx^\dagger y=\frac{1}{2\pi}\int_{\mathbb{R}}d\omega X^\dagger Y
> $$
> `\begin{proof}`
> Applichiamo la [[Trasformata di Fourier|trasformata]] alla funzione di [[Funzioni di crosscorrelazione e autocorrelazione|crosscorrelazione]]
> $$
> \dot\Phi_{x,y}(\omega)=\mathcal{F}[\dot\varphi_{x,y}(\tau)]=\mathcal{F}[x^\dagger(-\tau)]\mathcal{F}[y(\tau)]=X^\dagger(\omega)Y(\omega)
> $$
> ora che sappiamo che esiste la [[Trasformata di Fourier|trasformata]] della [[Funzioni di crosscorrelazione e autocorrelazione|crosscorrelazione]] scriviamola come sua antitrasformata
> $$
> \dot\varphi_{x,y}(\tau)=\frac{1}{2\pi}\int_{\mathbb{R}}d\omega\dot\Phi_{x,y}\e^{j\omega\tau}
> $$
> valutando la funzione in $\tau=0$ si ha
> $$
> \evals{\dot\varphi_{x,y}}{0}=\frac{1}{2\pi}\int_{\mathbb{R}}d\omega\dot\Phi_{x,y}=\frac{1}{2\pi}\int_{\mathbb{R}}d\omega X^\dagger Y
> $$
> allora applicando la definizione di [[Funzioni di crosscorrelazione e autocorrelazione|crosscorrelazione]] si ha
> $$
> \int_{\mathbb{R}}dtx^\dagger y=\frac{1}{2\pi}\int_{\mathbb{R}}d\omega X^\dagger Y
> $$
> `\end{proof}`

Il teorema di Parseval generalizzato consente di vedere se due segnali sono [[Rappresentazione ortonormale di segnali|ortogonali]] (utile per tecniche di multiplexing) osservando se le loro trasformate lo sono, perciò due segnali lo sono se:
* i due segnali non si sovrappongono nel tempo.
* i due segnali non si sovrappongono in frequenza.
* se invece due segnali si sovrappongono sia  nel tempo che in frequenza possono comunque essere  [[Rappresentazione ortonormale di segnali|ortogonali]].