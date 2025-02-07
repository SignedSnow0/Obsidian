---
subject: fondamenti di telecomunicazioni
---
> [!definition] Funzione di trasferimento
> Dato un sistema lineare $Q$ e la sua [[Risposta impulsiva|risposta impulsiva]] $h$ la sua funzione di trasferimento è
> $$
> H(\omega)=\mathcal{F}[h(t)]
> $$

Questa funzione permette di trovare la risposta del sistema nel dominio delle frequenze e nonostante sia più restrittiva della [[Risposta impulsiva|risposta impulsiva]] (richiede l'esistenza della trasformata), permette di trovarla usando le [[Proprietà della trasformata di Fourier|proprietà]] in maniera più immediata:
> [!theorem] Risposta nel dominio delle frequenze
> Dato un sistema lineare la sua risposta nelle frequenze è
> $$
> Y=XH
> $$
> `\begin{proof}`
> La risposta di un sistema lineare è
> $$
> y=x*h
> $$
> per le [[Proprietà della trasformata di Fourier|proprietà della trasformata si ha]]
> $$
> \mathcal{F}[y]=\mathcal{F}[x*h]=\mathcal{F}[x]\mathcal{F}[h]
> $$
> allora
> $$
> Y=XH
> $$
> `\end{proof}`

> [!remark] Definizione alternativa
> In alcuni casi è utile ricordare la definizione alternativa di funzione di trasferimento
> $$
> H=\frac{Y}{X}
> $$