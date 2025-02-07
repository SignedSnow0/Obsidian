---
subject: elettrotecnica
---
> [!theorem] Legge di Kirchhoff per le tensioni
> La somma di voltaggi entranti e uscenti da ogni [[Elementi circuitali|maglia]] è pari a $0$
> $$
> \sum v_i=0
> $$
> `\begin{proof}`
> Dalla [[Equazioni di Maxwell|terza equazione di Maxwell]] e dalle [[Ipotesi fondamentali della teoria dei circuiti|ipotesi dei circuiti]] si ha
> $$
> \oint\vec{E}\cdot d\vec{l}=-\oiint\frac{\partial\vec{B}}{\partial t}\cdot d\hat{S}=0
> $$
> perciò per ogni scomposizione della circuitazione si avrà che la somma delle parti sarà nulla. 
> `\end{proof}`

> [!theorem] Legge di Kirchhoff per le correnti
> La somma delle correnti entranti e uscenti da un [[Elementi circuitali|nodo]] è pari a $0$
> $$
> \sum i_k=0
> $$
> `\begin{proof}`
> Dalla [[Equazioni di Maxwell|prima equazione di Maxwell]] e dalle [[Ipotesi fondamentali della teoria dei circuiti|ipotesi dei circuiti]] si ha
> $$
> \iint_S\left(\vec{J}+\frac{\partial\vec{D}}{\partial t}\right)
\cdot d\hat{S}=\iint_S\vec{J}\cdot d\hat{S}=0
> $$
> allora per ogni nodo la somma delle correnti sarà nulla.
> `\end{proof}`