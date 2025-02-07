---
subject: fondamenti di telecomunicazioni
---
Il coefficiente SQNR (Signal to Quantization Noise Ratio) indica il rapporto fra la massima potenza del segnale trasmesso $x$ e la potenza dell'[[Conversione analogico - digitale con tecnica PCM|errore di quantizzazione]] $e$.
Iniziamo calcolando il coefficiente per ogni potenza trasmessa:
$$
\text{SQNR}=\frac{E\left[x^2\right]}{E\left[e^2\right]}
$$
utilizzando un [[Conversione analogico - digitale con tecnica PCM|quantizzatore]] lineare possiamo assumere che
* $x\sim U(-M,M)$
* $e\sim U\left(-\frac{q}{2},\frac{q}{2}\right)$

allora
$$
E[x^2]=\int_\mathbb{R}x^2p(x)dx=\frac{1}{2M}\int_{-M}^{M}x^2dx=\frac{1}{2M}\eval{\frac{x^3}{3}}{-M}{M}=\frac{M^2}{3}
$$

$$
E[e^2]=\int_\mathbb{R}e^2p(e)de=\frac{1}{q}\int_{-\frac{q}{2}}^{\frac{q}{2}}e^2de=\frac{1}{q}\eval{\frac{e^3}{3}}{-\frac{q}{2}}{\frac{q}{2}}=\frac{q^2}{12}
$$
dato che la risoluzione $q$ è pari all'intervallo di quantizzazione su il numero di bit disponibili
$$
q=\frac{2M}{L}=\frac{2M}{2^l}
$$
si ha
$$
E[e^2]=\frac{q^2}{12}=\frac{4M^2}{12\cdot4^l}
$$
allora
> [!definition] Rapporto SQNR per quantizzatore lineare
> $$
> \text{SQNR}=\frac{12M^2\cdot4^l}{12M^2}=4^l
> $$
---
In generale per un quantizzatore qualsiasi si ha
$$
\text{SQNR}=\frac{3\cdot 4^l\times E[x^2]}{M^2}
$$
dove $E[x^2]$ è la potenza del segnale trasmesso, e $M^2$ è la potenza massima del segnale, a volte semplificato con in rapporto potenza del segnale $P_x$, allora
> [!definition] Rapporto SQNR
> $$
> \text{SQNR}=3\cdot4^l\cdot P_x
> $$

allora in $dB$ si ha

> [!definition] Rapporto SQNR in dB
> $$
> \evals{\text{SQNR}}{dB}=10\log(\text{SQNR})=10\log3+20l\log2+\evals{P_x}{dB}\approx4.77\cdot6.02l+\evals{P_x}{dB}
> $$

perciò per ogni bit aggiunta in fase di [[Conversione analogico - digitale con tecnica PCM|campionamento]] il rapporto fra segnale ed errore diventa 6dB più forte.