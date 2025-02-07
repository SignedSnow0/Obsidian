> [!definition] Risonanza in serie
> ![lg](Risonanza.drawio.svg)
> ---
> Dato il seguente circuito la sua [[Impedenza|impedenza]] equivalente risulta
> $$
> \evec{Z}_{\text{eq}}=R+j\left(\omega L-\frac{1}{\omega C}\right)
> $$
> definendo la sua frequenza di risonanza come:
> $$
> \omega_0=\frac{1}{\sqrt{LC}}
> $$
> allora si ha
> $$
> \evals{\evec{Z}_{\text{eq}}}{\omega_0}=R
> $$
> perciò l'[[Induttori|induttore]] e [[Elettrotecnica/Componenti/Condensatori|condensatore]] non assorbono energia comportandosi come un corto circuito.

> [!definition] Risonanza in parallelo [Antirisonanza]
> ![lg](Antirisonanza.drawio.svg)
> ---
> Dato il seguente circuito la sua [[Impedenza|impedenza]] equivalente risulta
> $$
> \evec{Z}_{\text{eq}}=R+j\left(\frac{\omega L}{1-\omega^2LC}\right)
> $$
> definendo la sua frequenza di risonanza come:
> $$
> \omega_0=\frac{1}{\sqrt{LC}}
> $$
> allora si ha
> $$
> \evals{|\evec{Z}_{\text{eq}}|}{\omega_0}\to\infty
> $$
> perciò l'[[Induttori|induttore]] e [[Elettrotecnica/Componenti/Condensatori|condensatore]] in frequenza di risonanza assorbono tutta l'energia comportandosi come un circuito aperto.