---
subject: fondamenti di telecomunicazioni
---
La conversione analogica a digitale consiste di 3 fasi principali
 * Decodifica $q_n\to x_n$
 * Ricostruzione del segnale $x_n\to x$
 * Equalizzazione 
---
### Decodifica
La decodifica è il procedimento inverso della [[Conversione analogico - digitale con tecnica PCM|codifica]] e si occupa di tornare dalla parola scelta al valore $q_n$ originale.

---
### Ricostruzione del segnale
Il segnale di partenza è quello trasmesso con tecnica PAM ottenuto con convoluzione della [[Serie temporale|serie temporale]] e impulso rettangolare $g$
$$
s=\{x_n\}*g=\sum_{n=-\infty}^{+\infty}x_ng(t-nT)
$$
applicando la trasformata al segnale si ha 
$$
S=X_sG=\frac{1}{T}\sum_{k=-\infty}^{+\infty}X(\omega+k\omega_0)G
$$
se il segnale soddisfa le condizioni del [[Teorema di Shannon|teorema di Shannon]] non presenta aliasing e quindi è possible ottenere la funzione di partenza filtrando solo la prima ripetizione con un filtro passa-basso.
$$
S_f=X\frac{G}{T}
$$
---
### Equalizzazione
Dal passaggio precedente si ha il segnale originale moltiplicato per la trasformata dell'impulso rettangolare, passando il segnale per una rete lineare con [[Funzione di trasferimento|funzione di trasferimento]] 
$$
H=\frac{T}{G}\quad|\omega|\le\omega_m
$$
si ottiene il segnale di partenza.
Se l'impulso $g$ è sufficientemente piccolo la sua trasformata $G$ sarà grande abbastanza da poter essere approssimata costante nella banda $\omega_m$ del segnale $X$, perciò la fase di equalizzazione può essere omessa ottenendo un segnale di intensità maggiore.