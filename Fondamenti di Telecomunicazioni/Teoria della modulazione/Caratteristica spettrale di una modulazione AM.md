---
subject: fondamenti di telecomunicazioni
---
## Modulazione DSB
La [[Introduzione|portante modulata]] in AM è data da 
$$
s=V_0(1+kx)\cos\omega_0t
$$
allora il suo [[Inviluppo complesso rappresentativo|inviluppo complesso]] è dato da
$$
i=V_0(1+kx)
$$
che nel piano di Gauss è rappresentato sa una retta sull'asse reale positivo.
Separando i termini vediamo che il segnale è composto dalla portante e il prodotto della portante ed il segnale a meno di una costante $k$
$$
s=V_0\cos\omega_0t+kxV_0\cos\omega_0t
$$
Per ottenere la trasformata del segnale modulato iniziamo sostituendo $x$ con la sua trasformata ricordando che è puramente reale
$$
x=\int_{\omega_i}^{\omega_m}d\omega V\cos(\omega t-\phi)
$$
> [!definition] Segnale modulato DSB
> $$
> s=V_0\cos\omega_0t+\frac{kV_0}{2}\int_{\omega_i}^{\omega_m}d\omega V\cos((\omega_0+\omega)t-\phi)+\frac{kV_0}{2}\int_{\omega_i}^{\omega_m}d\omega V\cos((\omega_0-\omega)t+\phi)
> $$

da questa formula è possibile osservare che il segnale è dato da una frequenza portante, una banda laterale superiore ed una banda laterale inferiore, perciò il segnale AM è un tipo di segnale DSB (Double Sided Band).
Lo spettro dell'ampiezza è simmetrico rispetto alla frequenza della portante, la banda è pari a $B_\omega=2\omega_m$ dove $\omega_m$ è la pulsazione massima del segnale modulante. Lo spettro di fase è antisimmetrico rispetto alla frequenza portante. Se $\omega_m<<\omega_0$ allora $B_\omega<<\omega_0$ e l'oscillazione AM è un segnale passa banda.
Inoltre dall'espressione precedente è possibile dividere l'[[Inviluppo complesso rappresentativo|inviluppo complesso]] come somma di 3 parti: la prima che rappresenta l'onda portante e altre due che rappresentano le due bande simmetriche, perciò la prima parte è reale e positiva, mentre le altre due saranno complesse coniugate e positive per un totale reale e positivo.
> [!definition] Inviluppo complesso di un segnale DSB
> $$
> i=V_0+\frac{kV_0}{2}\int_{\omega_i}^{\omega_m}d\omega V\e^{j(\omega t-\phi)}+\frac{kV_0}{2}\int_{\omega_i}^{\omega_m}d\omega V\e^{-j(\omega t-\phi)}
> $$

---
## Modulazione SSB
Partendo dal segnale ottenuto dalla modulazione DSB notiamo che una delle due bande è recuperabile dall'altra, perciò eliminando una delle due bande si raddoppia la banda disponibile per la trasmissione e si ottiene un segnale SSB (Single Side Band).
Un modo per ottenere un segnale del genere è quello di partire da una normale modulazione AM passata poi per un filtro passa banda, il segnale e l'[[Inviluppo complesso rappresentativo|inviluppo complesso]] risultano
> [!definition] Segnale modulato SSB
> $$
> s=V_0\cos\omega_0t+\frac{kV_0}{2}\int_{\omega_i}^{\omega_m}d\omega V_0\cos((\omega_0+\omega)t-\phi)
> $$

> [!definition] Inviluppo complesso di un segnale SSB
> $$
> i=V_0+\frac{k\omega_0}{2}\int_{\omega_i}^{\omega_m}d\omega Ve^{j(\omega t-\phi)}
> $$
In questo caso il vettore rappresentativo totale diventa complesso generando quindi una modulazione ibrida.

---
## Modulazione DSB-SC
Sempre partendo dalla modulazione DSB, possiamo eliminare la portante ottenendo così un segnale di potenza inferiore con la stessa quantità di informazioni, la modulazione è la DSB-SC (DSB-Suppressed Carrier).
> [!definition] Segnale modulato DSB-SC
> $$
> s=\frac{kV_0}{2}\int_{\omega_i}^{\omega_m}d\omega V\cos((\omega_0+\omega)t-\phi)+\frac{kV_0}{2}\int_{\omega_i}^{\omega_m}d\omega V\cos((\omega_0-\omega)t+\phi)
> $$

> [!definition] Inviluppo complesso di un segnale DSB-SC
> $$
> i=\frac{kV_0}{2}\int_{\omega_i}^{\omega_m}d\omega V\e^{j(\omega t-\phi)}+\frac{kV_0}{2}\int_{\omega_i}^{\omega_m}d\omega V\e^{-j(\omega t-\phi)}
> $$
Il vettore rappresentativo dell'inviluppo pur essendo reale può essere sia positivo che negativo, quindi la modulazione rimane ibrida.

---
## Modulazione SSB-SC
Combinando gli accorgimenti della modulazione DSB-SC e SSB, si ottiene un segnale con entrambi i vantaggi chiamato SSB-SC (SSB-Suppressed Carrier).
> [!definition] Segnale modulato SSB-SC
> $$
> s=\frac{kV_0}{2}\int_{\omega_i}^{\omega_m}d\omega V\cos((\omega_0+\omega)t-\phi)
> $$

> [!definition] Inviluppo complesso di un segnale SSB-SC
> $$
> i=\frac{kV_0}{2}\int_{\omega_i}^{\omega_m}d\omega V\e^{j(\omega t-\phi)}
> $$

In questo caso la modulazione SSB-SC coincide con una conversione de frequenza in salita in quanto gli spettri di ampiezza e fase coincidono con quelli del segnale modulante.