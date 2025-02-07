> [!definition] Impedenza
> L'impedenza è un [[Fasore|fasore]] che indica il rapporto fra voltaggio e corrente
> $$
> \evec{Z}=\frac{\evec{V}}{\evec{I}}=\frac{V}{I}\e^{j(\varphi_V-\varphi_I)}
> $$
> possiamo notare che l'impedenza esprime il rapporto fra i due valori e il loro sfasamento.
> In forma algebrica è pari a
> $$
> \evec{Z}=Z_R+jZ_I
> $$
> * $Z_R$ è detta resistenza.
> * $Z_I$ è detta reattanza (espressa come $X$).

> [!definition] Ammettenza
> L'ammettenza è l'inverso dell'impedenza
> $$
> \evec{Y}=\frac{1}{\evec{Z}}=\frac{\evec{I}}{\evec{V}}=\frac{I}{V}\e^{j(\varphi_I-\varphi_V)}
> $$
---
> [!definition] Impedenza del resistore
> Dalle [[Equazioni costitutive|equazioni costitutive]] sappiamo che
> $$
> \evec{V}=R\evec{I}
> $$
> allora
> $$
> \evec{Z}=\frac{\evec{V}}{\evec{I}}=R
> $$
> perciò l'impedenza di un resistore non ha sfasamento ($\evec{Z}=R\e^0$) e ha solo resistenza ($\evec{Z}=R+j0$).

> [!definition] Impedenza del condensatore
> Dalle [[Equazioni costitutive|equazioni costitutive]] sappiamo che
> $$
> \evec{I}=j\omega C\evec{V}
> $$
> allora
> $$
> \evec{Z}=\frac{\evec{V}}{\evec{I}}=-j\frac{1}{\omega C}
> $$
> perciò il condensatore porta ad uno sfasamento di  $-\frac{\pi}{2}$ ($\evec{Z}=\frac{1}{\omega C}\e^{-j\frac{\pi}{2}}$) e l'impedenza è puramente reattiva ($\evec{Z}=0-j\frac{1}{\omega C}$).

> [!definition] Impedenza dell'induttore
> Dalle [[Equazioni costitutive|equazioni costitutive]] sappiamo che
> $$
> \evec{V}=j\omega L\evec{I}
> $$
> allora
> $$
> \evec{Z}=\frac{\evec{V}}{\evec{I}}=j\omega L
> $$
> perciò il condensatore porta ad uno sfasamento di  $\frac{\pi}{2}$ ($\evec{Z}=\omega L\e^{j\frac{\pi}{2}})$ e l'impedenza è puramente reattiva ($\evec{Z}=0+j\omega L$).