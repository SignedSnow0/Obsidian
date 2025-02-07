---
subject: fondamenti di telecomunicazioni
---
> [!definition] Potenza istantanea
> Dato un segnale $x$  si definisce potenza istantanea
> $$
> p=x^\dagger x=|x|^2
> $$

> [!definition] Energia
> Dato un segnale $x$ si definisce energia la potenza istantanea in ogni suo momento
> $$
> E=\int_{\mathbb{R}}dtx^\dagger x=\int_{\mathbb{R}}dt|x|^2 
> $$
> Un segnale ha energia finita se $E\in\mathbb{R}$.
> L'energia di un segnale è pari alla funzione di [[Funzioni di crosscorrelazione e autocorrelazione|autocorrelazione]] calcolata in $\tau=0$

> [!definition] Potenza
> Dato un segnale $x$ si definisce potenza l'energia media in un intervallo
> $$
> P=\langle x,x\rangle=\lim_{T\to+\infty}\frac{1}{T}\int_{-\frac{T}{2}}^{\frac{T}{2}}dtx^\dagger x=\lim_{T\to+\infty}\frac{1}{T}\int_{-\frac{T}{2}}^{\frac{T}{2}}dt|x|^2
> $$
> Un segnale ha potenza finita se $P\in\mathbb{R}\setminus\{0\}$

> [!definition] Valore efficace
> Se un segnale ha potenza finita si può definire il valore efficace come una potenza che se costante ha lo stesso valore del segnale
> $$
> x_{eff}=\sqrt{P}
> $$
 
Si noti che se un segnale ha potenza finita, allora avrà potenza pari a $0$, perciò un segnale non può avere sia energia che potenza finita.