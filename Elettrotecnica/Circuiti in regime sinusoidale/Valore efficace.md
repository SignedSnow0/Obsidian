> [!definition] Valore efficace
> Data una grandezza in [[Regime sinusoidale|regime sinusoidale]] il suo valore efficace è pari a:
> $$
> X=\frac{\hat{X}}{\sqrt{2}}
> $$
> `\begin{proof}`
> Partiamo dalla definizione di [[Regime sinusoidale|valore efficace]]
> $$
> X=\sqrt{\frac{1}{T}\int_Tdtx^2}=\sqrt{\frac{1}{T}\int_Tdt\hat{X}^2\cos^2(\omega t+\varphi)}
> $$
> $$
> =\sqrt{\frac{\hat{X}^2}{2}\int_Tdt\cos^2(\omega t+\varphi)}
> $$
> dato che l'integrale di una funzione periodica sul periodo è pari a $0$ si ha
> $$
> X=\sqrt{\frac{\hat{X}^2}{2}}=\frac{\hat{X}}{\sqrt{2}}
> $$
> `\end{proof}`

> [!definition] Effetto Joule
> Il valore efficace è tale che se:
> $$
> i=\hat{I}\cos(\omega t+\varphi),\quad p=Ri^2
> $$
> allora la potenza media dissipata è 
> $$
> P=RI^2
> $$
> dove $I$ è il valore efficace
> `\begin{proof}`
> Iniziamo con la definizione di [[Regime sinusoidale|potenza media]]:
> $$
> P=\frac{1}{T}\int_Tdtp=\frac{1}{T}\int dtRi^2=R\frac{1}{T}\int_Tdti^2=RI^2
> $$
> `\end{proof}`