> [!definition] Circuito in analisi
> ![lg](Stella-Triangolo.drawio.svg)

> [!theorem] Trasformazione triangolo-stella
> $$
> R_1=\frac{R_BR_C}{R_A+R_B+R_C}
> $$
> $$
> R_2=\frac{R_AR_B}{R_A+R_B+R_C}
> $$
> $$
> R_2=\frac{R_AR_C}{R_A+R_B+R_C}
> $$
> `\begin{proof}`
> Iniziamo scrivendo le resistenze fra le combinazioni di punti nella configurazione a stella
> $$
> R_{\alpha,\beta}=R_1+R_2
> $$
> $$
> R_{\alpha,\gamma}=R_1+R_3
> $$
> $$
> R_{\beta,\gamma}=R_2+R_3
> $$
> facciamo lo stesso per la configurazione a triangolo
> $$
> R_{\alpha,\beta}'=\frac{R_B(R_A+R_C)}{R_A+R_B+R_C}
> $$
> $$
> R_{\alpha,\gamma}'=\frac{R_C(R_A+R_B)}{R_A+R_B+R_C}
> $$
> $$
> R_{\beta,\gamma}'=\frac{R_A(R_B+R_C)}{R_A+R_B+R_C}
> $$
> dato che vogliamo ottenere due circuiti equivalenti poniamo ogni $R=R'$, allora abbiamo un sistema lineare di 3 equazioni e 3 incognite
> $$
> \begin{cases}R_1+R_2=\frac{R_B(R_A+R_C)}{R_A+R_B+R_C}\\ R_1+R_3=\frac{R_C(R_A+R_B)}{R_A+R_B+R_C}\\ R_2+R_3=\frac{R_A(R_B+R_C)}{R_A+R_B+R_C}\end{cases}
> $$
> allora risolvendo il sistema otteniamo le equazioni desiderate.
> `\end{proof}`

> [!theorem] Trasformazione stella-triangolo
> $$
> R_A=\frac{R_1R_2+R_2R_3+R_1R_3}{R_1}
> $$
> $$
> R_B=\frac{R_1R_2+R_2R_3+R_1R_3}{R_3}
> $$
> $$
> R_C=\frac{R_1R_2+R_2R_3+R_1R_3}{R_2}
> $$
> `\begin{proof}`
> Seguendo il ragionamento della trasformazione opposta si ottiene lo stesso sistema, considerando le variabili della formazione a stella date si risolve per le variabili della formazione a triangolo.
>`\end{proof}`