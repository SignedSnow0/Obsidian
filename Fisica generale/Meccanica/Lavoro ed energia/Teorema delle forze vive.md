---
subject: fisica generale
type: definizione
---
Il teorema delle forze vive correla i concetti di [[Secondo principio della dinamica|forza]], [[Lavoro|lavoro]] ed [[Energia Cinetica|energia]].
Il lavoro compiuto dalla risultante delle forze che agiscono su un sistema meccanico qualunque, nel passaggio da una configurazione $A$ a un'altra $B$, è uguale alla corrispondente variazione dell'[[Energia cinetica|energia cinetica]] di tale sistema.
$$
L_{A,B}=K_B-K_A
$$
# Dimostrazione
Partiamo dal [[Secondo principio della dinamica|secondo principio della dinamica]] 
$$
\vec{F}=m\vec{a}=m\frac{d\vec{v}}{dt}
$$
applichiamo la definizione di [[Lavoro|lavoro]] 
$$
L_{A,B}=\int_A^B\vec{F}\cdot d\vec{l}=\int_A^Bm\frac{d\vec{v}}{dt}\cdot d\vec{l}
$$
ricordando che lo [[Spostamento|spostamento]] è la [[Velocità vettoriale|velocità]] per il tempo, quindi $d\vec{l}=\vec{v}dt$ si ha
$$
L_{A,B}=\int_A^Bm\frac{d\vec{v}}{dt}\cdot\vec{v}dt
$$
applicando le proprietà delle derivate e del prodotto scalare
$$
\vec{v}\cdot\frac{d\vec{v}}{dt}=\frac12\left(\frac{d\vec{v}}{dt}\cdot\vec{v}+\vec{v}\cdot\frac{d\vec{v}}{dt}\right)=\frac12\frac{d}{dt}(\vec{v}\cdot\vec{v})=\frac12\frac{d|\vec{v}|^2}{dt}
$$
perciò
$$
L_{A,B}=\int_A^Bm\frac12\frac{dv^2}{dt}dt=\frac12m\int_A^Bdv^2=\eval{\frac12mv^2}{A}{B}=\frac12mv_B^2-\frac12mv_A^2\quad\square
$$