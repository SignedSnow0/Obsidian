Dalla [[Formula di Lagrange|formula di Lagrange]] possiamo notare che i [[Sistema dinamico tempo continuo|movimenti]] sono composti da due parti dipendenti dallo stato e dall'ingresso.
> [!definition] Movimento libero
> Il movimento libero di un sistema è quello che il sistema seguirebbe se l'ingresso fosse nullo, cioè
> $$
> \vec{x}_l=\e^{\mathbf{A}(t-t_0)}\vec{x}_{t_0}
> $$
> $$
> \vec{y}_l=\mathbf{C}\e^{\mathbf{A}(t-t_0)}\vec{x}_{t_0}
> $$

> [!definition] Movimento forzato
> Il movimento forzato di un sistema è quello che il sistema seguirebbe se lo stato fosse nullo, cioè
> $$
> \vec{x}_f=\int_{t_0}^{t}d\tau\e^{\mathbf{A}(t-\tau)}\mathbf{B}\vec{u}d\tau
> $$
> $$
> \vec{y}_f=\mathbf{C}\int_{t_0}^{t}d\tau\e^{\mathbf{A}(t-\tau)}\mathbf{B}\vec{u}+\mathbf{D}\vec{u}
> $$

> [!definition] Movimento libero di una matrice diagonalizzabile
> Grazie alle [[Rappresentazioni equivalenti|rappresentazioni equivalenti]], spesso possiamo rappresentare il movimento libero con una matrice $\hat{\mathbf{A}}$ tale che essa sia [[Matrice diagonalizzabile|diagonalizzabile]], allora si ha
> $$
> \hat{x}_l=\e^{\hat{\mathbf{A}}(t-t_0)}\hat{x}_{t_0}=\sum_{k=0}^{+\infty}\frac{(\hat{\mathbf{A}}t)^k}{k!}\hat{x}_{t_0}=
> $$
> $$
> =\text{diag}\left\{\sum_{k=0}^{+\infty}\frac{(s_1t)^k}{k!},\dots,\sum_{k=0}^{+\infty}\frac{(s_nt)^k}{k!}\right\}\hat{x}_{t_0}=
> $$
> $$
> =\text{diag}\{\e^{s_1t},\dots,\e^{s_nt}\}\hat{x}_{t_0}
> $$
> allora
> $$
> \vec{x}_l=\mathbf{T}^{-1}\hat{x}_l=\mathbf{T}^{-1}\text{diag}\{\e^{s_1t},\dots,\e^{s_nt}\}\mathbf{T}\vec{x}_{t_0}
> $$
> $$
> \vec{y}_l=\mathbf{CT}^{-1}\text{diag}\{\e^{s_1t},\dots,\e^{s_nt}\}
> $$
> Se la matrice non è diagonalizzabile è possibile attenere una matrice nella *forma di Jordan* quasi diagonale, allora i movimenti liberi dello stato saranno della forma
> $$
> t^{\eta-1}\e^{s_it}
> $$
> dove $\eta$ è un intero compreso fra $1$ e la massima dimensione dei miniblocchi di Jordan associati a $s_i$.