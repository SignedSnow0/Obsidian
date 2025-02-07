---
subject: fondamenti di telecomunicazioni
---
> [!definition] Discrete Fourier Transform
> La trasformata di Fourier discreta è una variazione della [[Trasformata di Fourier|trasformata]] di [[Trasformata di una serie temporale|serie temporali]] dove i termini sono finiti, inoltre questa trasformata mette in relazione biunivoca due tuple del segnale e della trasformata.
> $$
> (x_0,\dots,x_{N-1})\iff(X_0,\dots,X_{N-1})
> $$
> La $k$-esima trasformata è data da
> $$
> X_k=\sum_{n=0}^{N-1}x_n\e^{-j\frac{2\pi}{N}nk}
> $$
> e l'$n$-esimo [[Serie temporale|campionamento]] è 
> $$
> x_n=\frac{1}{N}\sum_{k=0}^{N-1}X_k\e^{j\frac{2\pi}{N}nk}
> $$
> `\begin{proof}`
> Dimostriamo che
> $$
> x_n=\frac{1}{N}\sum_{q=0}^{N-1}X_q\e^{j\frac{2\pi}{N}nq}
> $$
> sostituiamo i termini $X_k$ con la loro definizione
> $$
> \frac{1}{N}\sum_{q=0}^{N-1}X_q\e^{j\frac{2\pi}{N}nq}=\frac{1}{N}\sum_{q=0}^{N-1}\sum_{k=0}^{N-1}x_k\e^{-j\frac{2\pi}{N}kq}\e^{j\frac{2\pi}{N}nq}=\frac{1}{N}\sum_{k=0}^{N-1}x_k\sum_{q=0}^{N-1}\e^{j\frac{2\pi}{N}q(n-k)}
> $$
> continuiamo sulla sommatoria si $q$
> $$
> \sum_{q=0}^{N-1}\e^{j\frac{2\pi}{N}q(n-k)}=\sum_{q=0}^{N-1}\left(\e^{j\frac{2\pi}{N}(n-k)}\right)^q
> $$
> che è una [[Serie geometrica|serie geometrica]] di parametro $\e^{j\frac{2\pi}{N}(n-k)}$, allora sarà uguale a
> $$
> \sum_{q=0}^{N-1}\left(\e^{j\frac{2\pi}{N}(n-k)}\right)^q=\begin{cases}\frac{1-\e^{j2\pi(n-k)}}{1-\e^{j\frac{2\pi}{N}(n-k)}}&n\ne k\\ N&n=k\end{cases}
> $$
> dato che l'esponenziale è un multiplo di una rotazione del fasore sarà sempre uguale ad $1$, perciò il totale sarà nullo, quindi
> $$
> \sum_{q=0}^{N-1}\left(\e^{j\frac{2\pi}{N}(n-k)}\right)^q=\begin{cases}0&n\ne k\\ N&n=k\end{cases}
> $$
> tornando all'espressione iniziale abbiamo quindi
> $$
> x_n=\frac{1}{N}\sum_{k=0}^{N-1}x_k\sum_{q=0}^{N-1}\e^{j\frac{2\pi}{N}q(n-k)}=\frac{1}{N}x_nN=x_n
> $$
> `\end{proof}`

> [!remark] Relazione fra trasformata continua e DFT
> Assumiamo di prendere $N$ [[Serie temporale|campioni]] dal segnale $x$ e otteniamo $N$ trasformate $X$ tramite DFT
> $$
> x_p=\sum_{i=-\infty}^{+\infty}x(t-iT_p)
> $$
> $$
> X_p=\sum_{i=-\infty}^{+\infty}X(\omega-i\omega_p)
> $$
> i periodi $T_p$ e $\omega_p$ sono legati da
> $$
> T_p\omega_p=2\pi N
> $$ 
> allora con $N$ campioni per periodo abbiamo che gli intervalli di campionamento sono pari a
> $$
> \Delta t=\frac{T_p}{N}=\frac{2\pi}{\omega_p}
> $$
> $$
> \Delta\omega=\frac{\omega_p}{N}=\frac{2\pi}{T_p}
> $$
> allora
> $$
> \Delta t\Delta\omega=\frac{2\pi}{N}
> $$

