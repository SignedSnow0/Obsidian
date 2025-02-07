> [!definition] Teorema di Parseval
> Il teorema di Parseval è un caso particolare del [[Teorema di Parseval generalizzato|teorema di Parseval generalizzato]] dove $x,y$ sono lo stesso segnale, allora si ha
> $$
> E_x=\int_{\mathbb{R}}d\omega \frac{\mathcal{F}[\dot\varphi_x]}{2\pi}
> $$
> `\begin{proof}`
> Applichiamo il [[Teorema di Parseval generalizzato|teorema di Parseval generalizzato]] alla stessa funzione
> $$
> E_x=\evals{\dot\varphi_x}{0}=\int_{\mathbb{R}}dtx^\dagger x=\frac{1}{2\pi}\int_{\mathbb{R}}d\omega X^\dagger X
> $$
> dato che 
> $$
> X^*X=|X|^2=\mathcal{F}[\dot\varphi_x]
> $$
> si ha 
> $$
> E_x=\int_{\mathbb{R}}d\omega\frac{\mathcal{F}[\dot\varphi_x]}{2\pi}
> $$
> `\end{proof}`

> [!definition] Densità spettrale bilatera di energia
> La funzione integranda del teorema di Parseval prende il nome di densità bilatera spettrale di energia
> $$
> E_{\text{bil}}=\frac{\mathcal{F}[\dot\varphi_x]}{2\pi}=\frac{|X|^2}{2\pi}
> $$

> [!definition] Densità spettrale monolatera di energia
> Data la densità spettrale bilatera di energia si ottiene la monolatera
> $$
> E=\begin{cases}E_{\text{bil}}&\omega=0\\2E_{\text{bil}}&\omega>0\end{cases}
> $$
> l'energia è quindi ottenibile integrando il solo semiasse positivo
> $$
> E_x=\int_{0}^{+\infty}d\omega E
> $$
> infine, se si vuole ottenere l'energia in un intervallo di frequenze si può ricavare con
> $$
> E_{\omega_1,\omega_2}=\int_{\omega_1}^{\omega_2}d\omega E
> $$