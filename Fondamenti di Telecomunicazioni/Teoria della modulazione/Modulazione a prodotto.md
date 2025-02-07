---
subject: fondamenti di telecomunicazioni
---
> [!definition] Modulazione
> La modulazione a prodotto può essere ottenuta facendo il prodotto del [[Introduzione|segnale modulante]] per una sinusoide con un circuito chiamato mixer, ottenendo
> $$
> s=x\cos\omega_0t
> $$
> l'[[Inviluppo complesso rappresentativo|inviluppo complesso]] risulta quindi
> $$
> i=x
> $$
> e la modulazione risulta ibrida
> $$
> V=|x|
> $$
> $$
> \alpha=\begin{cases}0&x>0\\\pi&x<0\end{cases}
> $$
> lo spettro in frequenza è ottenibile dal [[Teorema fondamentale della modulazione|teorema fondamentale]]
> $$
> S=\frac{1}{2}X(\omega-\omega_0)+\frac{1}{2}X(\omega+\omega_0)
> $$
> infine il coefficiente di efficienza è il rapporto della banda del segnale modulante e modulato
> $$
> \eta_f=\frac{B_x}{B_s}=\frac{\omega_m}{2\omega_m}=\frac{1}{2}
> $$

> [!definition] Demodulatore
> La demodulazione si ottiene moltiplicando la modulata per la portante
> $$
> u=2s\cos\omega_0t=2x\cos^2\omega_0t=x+x\cos2\omega_0t
> $$
> allora applicando un filtro passa basso si ottiene
> $$
> x_d=x
> $$
> perciò il demodulatore è ottenuto da un modulatore a prodotto e un filtro passa basso.
> Un demodulatore reale impiega del tempo per operare, perciò utilizzerà una versione della portante fuori fase, perciò il segnale reale sarà
> $$
> u=2s\cos(\omega_0t-\Delta)=2x\cos\omega_0t\cos(\omega_0t-\Delta)=x\cos\Delta+x\cos(2\omega_0t-\Delta)
> $$
> e con un filtro passa basso si ha
> $$
> x_d=x\cos\Delta
> $$
> perciò il segnale reale risulterà attenuato di un valore $\cos\Delta$