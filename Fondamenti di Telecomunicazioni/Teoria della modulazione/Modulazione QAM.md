---
subject: fondamenti di telecomunicazioni
---
La modulazione QAM è un'estensione della [[Modulazione a prodotto|modulazione a prodotto]], consiste di due modulazioni a prodotto con la seconda [[Introduzione|portante]] sfasata in anticipo di $\frac{\pi}{2}$.

> [!definition] Modulazione
> I due segnali [[Introduzione|modulanti]] $x_1$ e $x_2$ vengono moltiplicati ognuno per una portante:
> $$
> s=x_1\cos\omega_0t-x_2\sin\omega_0t
> $$
> l'[[Inviluppo complesso rappresentativo|inviluppo complesso]] è
> $$
> i=x_1+jx_2
> $$
> perciò la modulazione sarà ibrida e l'efficienza risulta doppia
> $$
> \eta_f=\frac{2B_x}{B_s}=\frac{2\omega_m}{2\omega_m}=1
> $$

> [!definition] Demodulazione
> Il demodulatore è la somma di due [[Modulazione a prodotto|demodulatori a prodotto]], il segnale in uscita al primo demodulatore è
> $$
> u_p=2s\cos\omega_0t=2x_1\cos^2\omega_0t-2x_2\sin\omega_0t\cos\omega_0t=x_1+x_1\cos2\omega_0t-x_2\sin2\omega_0t
> $$
> applicando un filtro passa basso al primo termine si ha
> $$
> x_{pd}=x_1
> $$
> il secondo demodulatore opera in maniera analoga
> $$
> u_q=-2s\sin\omega_0t=2x_2\sin^2\omega_0t-2x_1\sin\omega_0t\cos\omega_0t=x_2-x_2\cos2\omega_0t-x_1\sin2\omega_0t
> $$
> con un filtro passa basso si ha
> $$
> x_{qd}=x_2
> $$
> In questo caso una demodulazione reale porta a dei segnali pari a
> $$
> x_{pd}=x_1\cos\Delta-x_2\sin\Delta
> $$
> $$
> x_{qd}=x_2\cos\Delta+x_1\sin\Delta
> $$
> perciò in questo caso una demodulazione reale porta non solo ad un'attenuazione dei segnali, ma anche ad un interferenza fra i due, inoltre se $\Delta=\frac{\pi}{2}$ i due segnali si invertono.