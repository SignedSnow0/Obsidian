---
subject: fisica generale
type: definizione
---
Dalle [[Leggi di Keplero|leggi di Keplero]] e dai principi di Newton si può derivare la legge di gravitazione universale:
Nel caso particolare di un cerchio di raggio $r$ abbiamo che la superficie $S$ coperta da uno spostamento $l$ è  
$$
\Delta S=\frac12r\Delta l
$$
allora 
$$
A(t)=\lim_{\Delta t\to0}\frac{\Delta S}{\Delta t}=\lim_{\Delta t\to0}\frac12r\frac{\Delta l}{\Delta t}=\frac12rv
$$
dato che l'area di una superficie è rappresentabile come un prodotto vettoriale si ha che la velocità areolare vettoriale è
$$
\vec{A}=\frac12\vec{r}\wedge\vec{v}\quad\left[L^2T^{-1}\right]
$$
che rispetta la [[Leggi di Keplero|prima legge di Keplero]], perchè il moto avviene su un piano.
Usando ora la [[Leggi di Keplero|seconda legge di Keplero]] sappiamo che
$$
\frac{d\vec{A}}{dt}=k
$$
quindi
$$
\frac{d\vec{A}}{dt}=\frac12\frac{d}{dt}(\vec{r}\wedge\vec{v})=\frac12\left(\frac{d\vec{r}}{dt}\wedge\vec{v}+\vec{r}\wedge\frac{d\vec{v}}{dt}\right)=\frac12\vec{r}\wedge\vec{a}=\vec{0}
$$
allora si avrà per forza che $\vec{r}\parallel\vec{a}$, quindi l'accelerazione è solo normale e il moto sarà circolare uniforme, dal [[Secondo principio della dinamica|secondo principio della dinamica]] abbiamo che 
$$
\vec{F}=m\vec{a}=F\hat{u}_r
$$
perciò abbiamo un [[Campo centrale|campo centrale]].
Sappiamo quindi che la velocità del moto è
$$
v=\frac{2\pi R}{T}
$$
Perciò 
$$
\vec{F}=m\vec{a}=m\vec{a}_n=-m\frac{\vec{v}^2}{R}\hat{u}_n=-m\frac{4\pi^2}{T^2}R\hat{u}_n
$$
dalla [[Leggi di Keplero|terza legge di Keplero]] si ha che $T^2=kR^3$, perciò
$$
\vec{F}=-m\frac{4\pi^2}{kR^2}\hat{u}_r
$$
infine raccogliendo $GM=\frac{4\pi^2}{k}$ si ha 
$$
\vec{F}=-G\frac{mM}{r^2}\hat{u}_r
$$
che è la legge di gravitazione universale.
Dati sperimentali indicano che
$$
G=6,672\times10^{-11}\ \frac{Nm^2}{kg^2}
$$