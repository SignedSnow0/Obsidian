---
subject: fondamenti di telecomunicazioni
---
In un sistema lineare si dice che non presenta distorsioni se il segnale in uscita differisce per una costante moltiplicativa e un ritardo
> [!definition] Segnale non distorto
> $$
> y(t)=Ax(t-t_0)
> $$

allora nella [[Trasformata di Fourier|trasformata]] si ha
$$
Y=AX\e^{-j\omega t_0}
$$
perciò la [[Funzione di trasferimento|funzione di trasferimento]] è 
$$
H=A\e^{-j\omega t_0}
$$
Notiamo che la condizione dipende dal segnale in ingresso, inoltre se $x$ sarà reale risulteranno reali anche $y$ e $A$, allora definendo $T_0=A$ si hanno le seguenti condizioni di non distorsione
> [!definition] Segnale reale non distorto
> $$
> \begin{cases}T=T_0\\\beta=\omega t_0\end{cases}\quad\forall|\omega|\in B_x
> $$
> Dove $B_x$ è la banda del segnale in ingresso $x$