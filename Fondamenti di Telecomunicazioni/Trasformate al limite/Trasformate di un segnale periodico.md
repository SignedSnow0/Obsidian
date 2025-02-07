---
subject: fondamenti di telecomunicazioni
---
Sono riportati i valori di trasformate di frequenza nulla $f_0=0$, frequenza singola $f_0$ e analoghi valori in termini di velocità angolare.

> [!definition] Trasformata di una costante
> $$
> \mathcal{F}_f[1]=\delta
> $$
> $$
> \mathcal{F}[1]=2\pi\delta
> $$
> `\begin{proof}`
> Applichiamo il [[Delta di Dirac|delta di Dirac]] all'[[Trasformata di Fourier|antitrasformata]]
> $$
> \int_\mathbb{R}df\delta e^{j2\pi ft}=\e^{0}
> $$
> `\end{proof}`

> [!definition] Trasformata di un fasore
> $$
> \mathcal{F}_f[\e^{j2\pi f_0t}]=\delta_{f_0}
> $$
> $$
> \mathcal{F}[\e^{j\omega_0t}]=2\pi\delta_{\omega_0}
> $$
> `\begin{proof}`
> Applichiamo il [[Delta di Dirac|delta di Dirac]] all'[[Trasformata di Fourier|antitrasformata]]
> $$
> \int_\mathbb{R}df\delta_{f_0}\e^{j2\pi ft}=\e^{j2\pi f_0t}
> $$
> `\end{proof}`

---
Usando le trasformate sopra riportate possiamo definire la [[Trasformata di Fourier|trasformata]] di un [[Forma esponenziale di segnali complessi|segnale periodico]]
> [!definition] Trasformata di una serie di Fourier
> $$
> X=\sum_{n=-\infty}^{+\infty}c_n2\pi\delta_{n\omega_0}
> $$
> $$
> X_f=\sum_{n=-\infty}^{+\infty}c_n\delta_{nf_0}
> $$