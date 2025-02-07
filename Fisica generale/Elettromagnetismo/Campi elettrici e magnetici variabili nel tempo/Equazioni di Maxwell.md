---
subject: fisica generale
type: definizione
---
Le equazioni di Maxwell sono le leggi fondamentali dell'elettromagnetismo, a partire da esse è possibile ricavare ogni legge elettromagnetica conosciuta, inoltre da esse si ricava che il campo elettrico e magnetico sono due facce della stessa medaglia, il campo elettromagnetico.
> [!definition] Leggi di Maxwell in forma differenziale
> 1. $$
> \vec{\nabla}\cdot\vec{E}=\frac{\rho}{\epsilon_0}
> $$
> 2. $$
> \vec{\nabla}\cdot\vec{B}=0
> $$
> 3. $$
> \vec{\nabla}\wedge\vec{E}=-\frac{\partial\vec{B}}{\partial t}
> $$
> 4. $$
> \vec{\nabla}\wedge\vec{B}=\mu_0\left(\vec{J}+\epsilon_0\frac{\partial{\vec{E}}}{\partial t}\right)
> $$

> [!definition] Leggi di Maxwell in forma integrale
> 1. $$
> \oiint_{\partial V}\vec{E}\cdot d\hat{S}=\frac{1}{\epsilon_0}\iiint_VpdV
> $$
> 2. $$
> \oiint\vec{B}\cdot d\hat{S}=0
> $$
> 3. $$
> \oint_\Gamma\vec{E}\cdot d\vec{l}=-\frac{d}{dt}\iint_{S_\Gamma}\vec{B}\cdot d\hat{S}
> $$
>  4. $$
> \oint_\Gamma\vec{B}\cdot d\vec{l}=\mu_0\left(\iint_{S_\Gamma}\vec{J}\cdot d\hat{S}+\epsilon_0\iint_{S_\Gamma}\frac{\partial\vec{E}}{\partial t}\cdot d\hat{S}\right)
> $$