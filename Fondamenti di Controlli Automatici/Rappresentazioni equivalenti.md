> [!definition] Rappresentazioni equivalenti
> Dato uno stato $\vec{x}$ è possibile esprimere le stesse informazioni con valori diversi, per ottenere la corrispondenza fra i due stati si può moltiplicare $x$ per una matrice costante, allora
> $$
> \hat{x}=\mathbf{T}\vec{x}
> $$
> inoltre visto che $\mathbf{T}$ è [[Invertibilità di una matrice|invertibile]] si ha
> $$
> \vec{x}=\mathbf{T}^{-1}\hat{x}
> $$
> allora le equazioni di movimento diventano
> $$
> \frac{d\hat{x}}{dt}=\hat{\mathbf{A}}\hat{x}+\hat{\mathbf{B}}\vec{u}
> $$
> $$
> \vec{y}=\hat{\mathbf{C}}\hat{x}+\hat{\mathbf{D}}\vec{u}
> $$
> con 
> * $\hat{\mathbf{A}}=\mathbf{TAT}^{-1}$ 
> * $\hat{\mathbf{B}}=\mathbf{TB}$
> * $\hat{\mathbf{C}}=\mathbf{CT}^{-1}$
> * $\hat{\mathbf{D}}=\mathbf{D}$
>
> `\begin{proof}`
> Scriviamo le equazioni di movimento ricordando la definizione di $\hat{x}$:
> $$
> \frac{d\vec{x}}{dt}=\mathbf{AT}^{-1}\hat{x}+\mathbf{B}\vec{u}
> $$
> ricordiamo che $\mathbf{TT}^{-1}=I$
> $$
> \mathbf{T}^{-1}\mathbf{T}\frac{d\vec{x}}{dt}=\mathbf{AT}^{-1}\hat{x}+\mathbf{B}\vec{u}
> $$
> spostiamo $\mathbf{T}^{-1}$ è raccogliamo $T\vec{x}=\hat{x}$
> $$
> \mathbf{T}\frac{d\vec{x}}{dt}=\mathbf{TAT}^{-1}\hat{x}+\mathbf{TB}\vec{u}
> $$
> allora
> $$
> \frac{d\hat{x}}{dt}=\hat{\mathbf{A}}\hat{x}+\hat{\mathbf{B}}\vec{u}
> $$
> e in maniera analoga
> $$
> \vec{y}=\hat{\mathbf{C}}\hat{x}+\hat{\mathbf{D}}\vec{u}
> $$
> `\end{proof}`

> [!remark] Similarità
> Dato che $\hat{\mathbf{A}}=\mathbf{TAT}^{-1}$, allora $\mathbf{A}$ e $\mathbf{A}^{-1}$ sono [[Matrici simili|simili]], allora hanno gli stessi [[Autovalore e autovettore di una matrice|autovalori]].