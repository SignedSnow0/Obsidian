---
subject: fondamenti di telecomunicazioni
---
Per calcolare la [[Risposta impulsiva|risposta impulsiva]] definiamo l'impulso come il limite di una funzione che soddisfa la [[Delta di Dirac|distribuzione di Dirac]]
$$
h=\lim_{\Delta\to0}y_\Delta
$$
il circuito RC ha in uscita i seguenti valori
$$
y_{\Delta}=\begin{cases}0&t<0\\\frac{1}{\Delta}\left(1-\e^{-\frac{t}{RC}}\right)&0\le t\le\Delta\\\frac{1}{\Delta}\left(1-\e^{-\frac{\Delta}{RC}}\right)\e^{-\frac{t-\Delta}{RC}}&t\ge\Delta\end{cases}
$$
prendendo quindi il limite di $\Delta\to0$ si ha che la parte centrale del sistema non si presenta, inoltre per la parte finale ricordiamo il limite dallo [[Sviluppo di Taylor con resto di Peano|sviluppo di Taylor]]
$$
\lim_{x\to0}\e^{x}=1+x
$$
perciò
$$
h=\lim_{\Delta\to0}y=\begin{cases}0&t<0\\\frac{1}{RC}\e^{-\frac{t}{RC}}&t\ge0\end{cases}
$$
infine la funzione di trasferimento è
$$
H=\frac{1}{1+j\omega RC}
$$