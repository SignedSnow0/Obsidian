---
subject: fondamenti di telecomunicazioni
---
In maniera equivalente alla [[Rappresentazioni monolatere di segnali reali|rappresentazione monolatera per segnali periodici]] si ha che la [[Trasformata di Fourier|trasformata di Fourier]] per segnali reali gode di simmetria hermitiana:
> [!remark] Simmetria hermitiana
> $$
> X(-\omega)=X^*(\omega)
> $$

allora si ha procedendo in maniera equivalente al caso periodico si ha
> [!definition] Rappresentazione per fasori
> $$
> x=\frac{1}{2\pi}\int_0^{+\infty}d\omega2\Re\left\{|X|\e^{j\arg\{X\}}\e^{j\omega t}\right\}
> $$

Passando alla rappresentazione trigonometrica si ha 
$$
x=\int_0^{+\infty}d\omega\frac{|X|}{\pi}\cos(\arg\{X\}+\omega t)
$$
allora, definendo lo spettro di ampiezza  e fase come
$$
V=\frac{|X|}{\pi}
$$
$$
\phi=-\angle X
$$
si ha l'integrale di Fourier
> [!definition] Integrale di Fourier
> $$
> x=\int_0^{+\infty}d\omega V\cos(\omega t-\phi)
> $$
