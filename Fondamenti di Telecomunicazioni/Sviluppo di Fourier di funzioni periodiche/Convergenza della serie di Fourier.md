---
subject: fondamenti di telecomunicazioni
---
Esistono due tipi principali convergenza per le serie di Fourier:
> [!definition] Convergenza puntuale
> $$
> \lim_{N\to\infty}\left\{x-\sum_{n=-N}^{N}c_n\e^{jn\omega_0t}\right\}=0
> $$

Per far si che una serie converga puntualmente sono necessarie tre condizioni chiamate condizioni di Dirichelet
1. $x$ è assolutamente integrabile, cioè $\int_0^Tdt|x|<+\infty$
2. Il numero di picchi nella parte reale ed immaginaria in un periodo è finito
3. Il segnale $x$ è continuo o possiede un numero finito di discontinuità di prima specie.
---
> [!definition] Convergenza media quadratica
> La serie di Fourier di un segnale esiste se esso ha [[Energia e potenza di un segnale|energia finita]], allora convergerà in media quadratica, cioè
> $$
> \lim_{N\to\infty}\int_0^Tdt\left|x-\sum_{n=-N}^{N}c_n\e^{jn\omega_0t}\right|^2=0
> $$