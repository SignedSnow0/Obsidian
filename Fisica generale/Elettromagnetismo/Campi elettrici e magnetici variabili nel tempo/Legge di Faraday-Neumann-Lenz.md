---
subject: fisica generale
type: definizione
---
La legge di Faraday-Neummann-Lenz descrive come il campo magnetico possa produrre una [[Forza elettromotrice|forza elettromotrice]]
$$
\mathcal{E}_{\text{ind}}=-\frac{d}{dt}\iint\vec{B}\cdot d\hat{S}=-\frac{d\Phi_S(\vec{B})}{dt}
$$
La legge detta che la variazione di flusso del campo magnetico crea una forza [[Forza elettromotrice|forza elettromotrice]] che si oppone alla variazione del flusso che l'ha creata, in modo di garantire conservazione dell'energia.

Applicando il [[Formula di Stokes|teorema di Stokes]] alla definizione di [[Forza elettromotrice|forza elettromotrice]] si ha
$$
\mathcal{E}=\oint_\Gamma\vec{E}\cdot d\vec{l}=\iint_{S_\Gamma}\vec\nabla\wedge\vec{E}\cdot d\hat{S}
$$
combinando il risultato con la legge di Faraday-Neumann-Lenz si ha
$$
\mathcal{E}=\iint_{S_\Gamma}\vec\nabla\wedge\vec{E}\cdot d\vec{S}=-\frac{d}{dt}\iint_{S_\Gamma}\vec{B}\cdot d\hat{S}=\iint_{S_\Gamma}-\frac{\partial\vec{B}}{\partial t}\cdot d\hat{S}
$$
arrivando alla forma locale della legge
$$
\vec\nabla\wedge\vec{E}=-\frac{\partial\vec{B}}{\partial t}
$$
---
Consideriamo un sistema formato da due fili conduttori paralleli e connessi, poniamo una barretta conduttrice ortogonale ai binari, in contatto con essi e in movimento lungo i binari con velocità costante, allora se il sistema è in un campo magnetico ortogonale al piano del circuito è presente una forza simile alla [[Forza elettromotrice|forza elettromotrice]], cerchiamo di determinarne la causa.

Secondo la [[Forza di Lorentz|forza di Lorentz]] le cariche libere nella barretta sentono una forza che le fa scorrere nel circuito verso l'alto.
$$
\vec{F}=q_e\vec{v}\wedge\vec{B}
$$
allora le cariche in un tratto $d\vec{l}$ è come se fossero soggette ad una [[Forza elettromotrice|forza elettromotrice]]
$$
d\mathcal{E}=\vec{E}\cdot d\vec{l}=\frac{\vec{F}}{q_e}\cdot d\vec{l}=\vec{v}\wedge\vec{B}\cdot d\vec{l}
$$
ricordando che la velocità è il rapporto tra distanza e tempo si ha
$$
d\mathcal{E}=\vec{v}\wedge\vec{B}\cdot d\vec{l}=\frac{d\vec{x}}{dt}\wedge\vec{B}\cdot d\vec{l}=d\vec{l}\wedge\frac{d\vec{x}}{dt}\cdot\vec{B}=\frac{d}{dt}\left[\left(d\vec{l}\wedge d\vec{x}\right)\cdot\vec{B}\right]
$$
Notiamo che $d\vec{l}\wedge d\vec{x}=-d\hat{S}$, allora
$$
d\mathcal{E}=-\frac{d}{dt}\left[\vec{B}\cdot d\hat{S}\right]
$$
perciò
$$
\mathcal{E}=-\frac{d}{dt}\iint_S\vec{B}\cdot d\hat{S}=-\frac{d\Phi_S(\vec{B})}{dt}
$$