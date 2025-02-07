---
subject: fondamenti di telecomunicazioni
---
Dato un sistema lineare tempo invariante, la risposta $h$ al'impulso del [[Delta di Dirac|delta di Dirac]] permette di esprimere la risposta di un qualsiasi segnale $x$
> [!theorem] Risposta impulsiva
> Dato un qualsiasi segnale $x$, la sua risposta $y$ sarà:
> $$
> y=x*h
> $$
> `\begin{proof}`
> La risposta al [[Delta di Dirac|delta di Dirac]] è
> $$
> Q[\delta]=h
> $$
> per tempo invarianza si ha
> $$
> Q[\delta(t-\tau)]=h(t-\tau)
> $$
> per linearità si ha
> $$
> Q[x(\tau)\delta(t-\tau)]=x(\tau)Q[\delta(t-\tau)]=x(\tau)h(t-\tau)
> $$
> allora si ha
> $$
> \int_\mathbb{R}d\tau x(\tau)\delta(t-\tau)=\int_\mathbb{R}d\tau x(\tau)h(t-\tau)
> $$
> $$
> x*\delta=x*h
> $$
> dato che il [[Delta di Dirac|delta di Dirac]] è l'[[Proprietà del delta di Dirac|elemento neutro della convoluzione]]
> $$
> x=x*h
> $$
> `\end{proof}`