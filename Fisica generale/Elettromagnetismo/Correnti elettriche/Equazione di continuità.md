---
subject: fisica generale
type: definizione
---
Consideriamo le formule della [[Intensità di corrente|intensità]] e [[Densità di corrente|densità]] di corrente per una superficie chiusa:
* Dalla [[Densità di corrente|densità]] di corrente sappiamo che l'intensità è calcolata con
$$
i=\oiint\vec{J}\cdot d\hat{S}
$$
* Dall'[[Intensità di corrente|intensità]] di corrente sappiamo che 
$$
i=-\frac{dq}{dt}
$$

Allora si ha che
$$
\oiint\vec{J}\cdot d\hat{S}=-\frac{dq}{dt}
$$
ciò significa che l'unica variazione di carica possibile in un sistema chiuso è dato da cariche che entrano o escono dalla superficie del sistema, quindi la carica non può essere creata o distrutta ottenendo così il principio di conservazione della carica.
Inoltre applicando il [[Teorema della divergenza|teorema della divergenza]] si ha 
$$
\vec\nabla\cdot\vec{J}=-\frac{\partial\rho}{\partial t}
$$
ottenendo l'equazione di continuità che dice che la divergenza della densità di corrente bilancia la variazione di carica.
$$
\vec\nabla\cdot\vec{J}+\frac{\partial\rho}{\partial t}=0
$$
mentre in condizioni stazionarie, quindi di elettrostatica si ha che il flusso della corrente è nullo e quindi il campo della densità di corrente è solenoidale
$$
\vec\nabla\cdot\vec{J}=0
$$