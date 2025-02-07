> [!definition] Potenza attiva e reattiva
> In un circuito in regime sinusoidale la potenza istantanea è divisa in due componenti
> $$
> p=\hat{V}\hat{I}\cos^2(\omega t)\cos(\varphi)+\hat{V}\hat{I}\cos(\omega t)\sin(\omega t)\sin(\omega t)
> $$
> $$
> =2VI\cos^2(\omega t)\cos(\varphi)+VI\sin(2\omega t)\sin(\varphi)
> $$
> dove la prima componente è chiamata potenza attiva istantanea e la seconda potenza reattiva istantanea.
> `\begin{proof}`
> In regime sinusoidale il voltaggio e corrente sono dati da:
> $$
> v=\hat{V}\cos(\omega t+\alpha_v)
> $$
> $$
> i=\hat{I}\cos(\omega t+\alpha_i)
> $$
> esprimendo $i$ in termini di differenze con $v$ si ha
> $$
> i=\hat{I}\cos(\omega t-\varphi)
> $$
> dove $\varphi=\alpha_v-\alpha_i$.
> Dividiamo allora $i$ in due componenti grazie alle formule trigonometriche: una in fase con $v$ e l'altra in quadratura
> $$
> i=i_a+i_f=\hat{I}\cos(\omega t)\cos(\varphi)+\hat{I}\sin(\omega t)\sin(\varphi)
> $$
> allora dato che $p=vi$ si ha
> $$
> p=vi_\alpha+vi_f=\hat{V}\cos(\omega t)\hat{I}\cos(\omega t)\cos(\varphi)+\hat{V}\cos(\omega t)+\hat{I}\sin(\omega t)\sin(\varphi)
> $$
> `\end{proof}`

> [!definition] Energia assorbita
> L'energia estraibile da un circuito in regime sinusoidale durante un periodo è pari a:
> $$
> E=TVI\cos\varphi
> $$
> `\begin{proof}`
> $$
> L=\int_0^Tdtp=\int_0^Tdt(p_a+p_f)=\int_0^Tdt2VI\cos\varphi\cos^2\omega t+\int_0^TdtVI\sin\varphi\sin2\omega t
> $$
> $$
> =2VI\cos\varphi\int_0^Tdt\cos^2\omega t=2VI\cos\varphi\int_0^Tdt\frac{1+\cos2\omega t}{2}=2VI\cos\varphi\frac{1}{2}T
> $$
> $$
> =TVI\cos\varphi
> $$
> `\end{proof}`

> [!definition] Potenza media
> La potenza media è pari a
> $$
> P=VI\cos\varphi
> $$

> [!definition] Potenza complessa
> La potenza complessa è un numero complesso che rappresenta entrambe le componenti della potenza istantanea in termini fasoriali
> $$
> \evec{N}=\evec{V}\evec{I}^\dagger=VI\e^{j\varphi}=VI\cos\varphi+jVI\sin\varphi
> $$
> dove la parte reale rappresenta la potenza attiva $P$ e la parte immaginaria rappresenta la potenza reattiva $Q$
> Inoltre applicando la legge di Ohm si ha
> $$
> \evec{N}=RI^2+jXI^2
> $$
> * $VI\cos\varphi$ è misurato in *Watt* (W)
> * $VI\sin\varphi$ è misurato in *voltampere reattivi* (VAr)
> * $\evec{N}$ è misurato in *voltampere* (VA)
