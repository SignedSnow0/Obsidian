---
subject: fondamenti di telecomunicazioni
---
Presa una [[Serie temporale|serie temporale]] ottenuta per campionamento in generale non è possibile ottenere il segnale di partenza perché esistono infinite funzioni che passano per i valori campionati.
Però noi sappiamo ottenere la [[Trasformata di Fourier|trasformata del segnale]] $X$ e la [[Trasformata di una serie temporale|trasformata della serie temporale]] $X_s$, e grazie al [[Serie temporale|lemma]] sappiamo che con $X$ possiamo ottenere $X_s$, però per il teorema di Shannon se la periodicità del segnale $X$ è abbastanza basso relativamente alla frequenza di campionamento è possibile ricavare $X$ a partire da $X_s$, permettendo quindi di trovare $x$ da $\{x_n\}$.
> [!theorem] Teorema di Shannon
> Data una [[Serie temporale|serie temporale]] $\{x_n\}$ ottenuta per campionamento, se la frequenza di campionamento $f_0$ è maggiore del doppio della frequenza massima del segnale ($f_m$ $f_0>2f_m$) si ha assenza di aliasing, allora è possibile ottenere il segnale di partenza $x$ a partire da $\{x_n\}$.
> Inoltre la frequenza massima rappresentabile è chiamata frequenza di Nyquist.