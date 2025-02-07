---
subject: fondamenti di telecomunicazioni
---
> [!theorem] Teorema fondamentale della modulazione
> Dato un [[Introduzione|segnale modulato]] 
> $$
> s=x\cos\omega_0t
> $$
> lo spettro di banda consiste nel segnale modulante duplicato e traslato di $\pm\omega_0$, cioè
> $$
> S=\frac{1}{2}X(\omega-\omega_0)+\frac{1}{2}X(\omega+\omega_0)
> $$
> `\begin{proof}`
> Ricordiamo che
> $$
> \cos\omega_0t=\frac{1}{2}\e^{j\omega_0t}+\frac{1}{2}\e^{-j\omega_0t}
> $$
> facciamo allora la [[Trasformata di Fourier|trasformata]] al [[Introduzione|segnale modulato]]
> $$
> S=\int_{\mathbb{R}}dtx\e^{-j\omega0t}=\frac{1}{2}\int_{\mathbb{R}}dtx\e^{j\omega_0t}\e^{j\omega t}+\frac{1}{2}\int_{\mathbb{R}}dtx\e^{-j\omega_0t}\e^{-j\omega t}
> $$
> $$
> =\frac{1}{2}\int_{\mathbb{R}}dtx\e^{-j(\omega-\omega_0)t}+\frac{1}{2}\int_{\mathbb{R}}dtx\e^{-j(\omega+\omega_0)t}
> $$
> $$
> =\frac{1}{2}X(\omega-\omega_0)+\frac{1}{2}X(\omega+\omega_0)
> $$
> `\end{proof}`