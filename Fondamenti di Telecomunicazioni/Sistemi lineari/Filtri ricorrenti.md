---
subject: fondamenti di telecomunicazioni
---
Un filtro ricorrente è una rete lineare composta da $N-1$ blocchi che ritardano in cascata il segnale ognuno di una quantità $T$ che viene poi moltiplicato per un coefficiente $h_n$ che formano il ramo diretto, poi viene aggiunta una seconda serie di $M$ blocchi simili con coefficienti $h_n'$ in retroazione con input il segnale in uscita, ottenuto dalla sommatoria di tutti i blocchi sia diretti che in retroazione.

> [!definition] Funzione di trasferimento di un filtro ricorrente
> $$
> H=\frac{\displaystyle \sum_{k=0}^{N-1}h_k\e^{-j\omega kt}}{\displaystyle1-\sum_{k=1}^{M}h_k'\e^{-j\omega kt}}
> $$
> `\begin{proof}`
> Il segnale in uscita $y$ è rappresentabile come
> $$
> y=\sum_{k=0}^{N-1}h_kx(t-kT)+\sum_{k=1}^{M}h_k'y(t-kT)
> $$
> applicando la [[Trasformata di Fourier|trasformata]] si ha
> $$
> Y=\sum_{k=0}^{N-1}h_kX\e^{-j\omega kT}+\sum_{k=1}^{M}h_k'\e^{-j\omega kT}
> $$
> allora con un po di manipolazione algebrica si ha
> $$
> H=\frac{Y}{X}=\frac{\displaystyle \sum_{k=0}^{N-1}h_k\e^{-j\omega kt}}{\displaystyle1-\sum_{k=1}^{M}h_k'\e^{-j\omega kt}}
> $$
> `\end{proof}`

---
Esistono poi anche i filtri trasversali dove manca il ramo in retroazione, e i filtri puramente ricorrenti con solo il ramo in retroazione.

> [!definition] Filtro trasversale
> Risposta impulsiva
> $$
> h=\sum_{k=0}^{N-1}h_k\delta_{kT}
> $$
> Funzione di trasferimento
> $$
> H=\sum_{k=0}^{N-1}h_k\e^{-j\omega kT}
> $$

> [!definition] Funzione di trasferimento di un filtro puramente ricorrente
> $$
> H=\frac{1}{\displaystyle 1-\sum_{k=1}^{M}h_k'\e^{-j\omega kt}}
> $$