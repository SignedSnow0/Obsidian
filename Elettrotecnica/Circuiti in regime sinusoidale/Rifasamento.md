![lg](Rifasamento1.drawio.svg)

In un sistema monofase reale la linea di trasmissione impone un'[[Impedenza|impedenza]] dovuta all'[[Effetto Joule|effetto Joule]] $\evec{Z}_l$ di tipo Ohmico-induttivo
$$
\evec{Z}_l=R_l-jX_l,\quad X_l>0
$$
Ciò porta ai seguenti effetti indesiderati:
1. Si ha una perdita di potenza lungo la linea di trasmissione pari a
$$
P_l=R_lI_l^2
$$
2. Si ha un calo di tensione che arriva al carico pari a
$$
\evec{V}'=\evec{V}-\evec{V}_l=\evec{V}-\evec{Z}_l\evec{I}_l
$$
---
Analizziamo la potenza attiva vista dall'utilizzatore:
$$
P_u=V_uI_u\cos\varphi\implies I_l=I_u=\frac{P_u}{V_u\cos\varphi}
$$
dato che per progetto del sistema $V_u,P_u$ sono fissi e aumentare $I_u$ porterebbe ad aumentare $I_l$ e di conseguenza peggiorare gli effetti negativi descritti, l'unica variabile modificabile per migliorare il rendimento è $\varphi$.

> [!definition] Rifasamento monofase
> ![lg](Rifasamento2.drawio.svg)
> Per diminuire gli sprechi di potenza lungo il trasporto di corrente si inserisce un carico capacitivo in parallelo al carico dell'utilizzatore vicino ad esso, allora si ha
> $$
> I_l'<I_l
> $$
> $$
> N'<N
> $$
> cioè il generatore nel nuovo sistema deve erogare meno corrente per ottenere lo stesso voltaggio lungo l'utilizzatore e la potenza complessa totale è inferiore (in particolare la potenza attiva è la stessa ma la potenza reattiva è fornita in parte dal condensatore.)
> 
> ---
> Per legge è obbligatorio che $\cos\varphi<0.95$ per evitare che il carico diventi capacitivo rischiando di danneggiare il circuito.

> [!definition] Valore di $C$
> $$
> C=\frac{P(\tan\varphi'-\tan\varphi)}{\omega V^2}
> $$
> `\begin{proof}`
> Dal grafico si vede che
> $$
> Q=P\tan\varphi
> $$
> $$
> Q'=P\tan\varphi'
> $$
> allora il condensatore deve fornire [[Elettrotecnica/Circuiti in regime sinusoidale/Potenza|potenza reattiva]] pari a
> $$
> Q_c=P(\tan\varphi'-\tan\varphi)
> $$
> inoltre sappiamo che
> $$
> Q_C=X_CI^2=-\frac{1}{\omega C}(\omega CV)^2=-\omega CV^2
> $$
> allora si ha
> $$
> -\omega CV^2=P(\tan\varphi'-\tan\varphi)\implies C=\frac{P(\tan\varphi-\tan\varphi')}{\omega V^2}
> $$
> `\end{proof}`
 
