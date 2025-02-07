``Il trasformatore monofase è una macchina elettrica utilizzata per modificare il voltaggio o corrente da una spira primaria alla secondaria.
È formato da un avvolgimento primario, un avvolgimento secondario e un nucleo [[Materiali magnetici|ferromagnetico]].
In generale un trasformatore ha un efficienza del 98% cioè
$$
P_2=\eta P_1\quad\eta\ge0,98
$$
Per raggiungere questi valori si utilizzato diverse tecniche:
* Per minimizzare il flusso che si richiude sulle spire  queste vengono disposte in due cilindri concentrici e poi avvolte nel nucleo (nucleo a mantello).
* Per minimizzare le perdite nel nucleo, si cercano di limitare le [[Legge di Faraday-Neumann-Lenz|correnti di induzione]] dividendo il nucleo in tante lamine isolate elettricamente.

> [!definition] Legge del trasformatore
> $$
> I_1N_1=I_2N_2\quad V_1N_2=V_2N_1
> $$
> dove $\frac{N_1}{N_2}=k$ è chiamato rapporto di trasformazione.
> `\begin{proof}`
> Consideriamo i [[Auto e mutua induzione|flussci concatenati]] delle due spire:
> Per la spira primaria sappiamo che il flusso è diviso in quello portato nel nucleo è quello disperso in se stessa:
> $$
> \Phi_{C1}=N_1\Phi+\Phi_{D1}
> $$
> il voltaggio invece è dato dalla [[Equazioni di Maxwell|terza legge di Maxwell]] e la [[Leggi di Ohm|legge di Ohm]]:
> $$
> v_1=\frac{\partial\Phi_{C1}}{\partial t}+R_1I_1=N_1\frac{\partial\Phi}{\partial t}+\frac{\partial\Phi_{D1}}{\partial t}+R_1I_1
> $$
> [[Auto e mutua induzione|sappiamo]] che la corrente dispersa è proporzionale alla corrente, quindi:
> $$
> v_1=N_1\frac{\partial\Phi}{\partial t}+L_{D,1}\frac{dI_1}{dt}+R_1I_1
> $$
> a sua volta il flusso nel nucleo è dato dai due coefficienti di induzione:
> $$
> v_1=N_1\left(L_1\frac{dI_1}{dt}+M_{1,2}\frac{dI_2}{dt}\right)+L_{D,1}\frac{dI_1}{dt}+R_1I_1
> $$
> quindi si ha
> $$
> v_1=L_1\frac{dI_1}{dt}+M\frac{dI_2}{dt}+L_{D,1}\frac{dI_1}{dt}+R_1I_1
> $$
> $v_2$ è ottenuta analogamente, ricordando i versi dei vettori e la convenzione dell'utilizzatore:
> $$
> v_2=L_2\frac{dI_2}{dt}+M\frac{dI_1}{dt}-L_{D,2}\frac{dI_2}{dt}-R_2I_2
> $$
> Per la corrente invece possiamo applicare l'[[LKT magnetica|LKT]] al circuito che [[Circuiti a parametri concentrati|rappresenta il trasformatore]]:
> $$
> N_1I_1-\psi-N_2I_2=0\implies N_1I_1-N_2I_2=\mathcal{R}\Phi
> $$
> che ci danno le due equazioni di un trasformatore reale.
> Se inoltre consideriamo un trasformatore ideale si ha 
> $$
> R_1=R_2=0\quad L_{D,1}=L_{D,2}=0\quad \mathcal{R}=0
> $$
> allora si hanno le formule cercate.
> `\end{proof}`