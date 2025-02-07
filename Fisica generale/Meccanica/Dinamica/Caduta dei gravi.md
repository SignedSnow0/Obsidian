---
subject: fisica generale
type: definizione
---
Studiamo in termini dinamici il [[Moto dei gravi|moto dei gravi]], sappiamo che l'unica accelerazione presente in questo moto è quella di gravità, esplicitiamo quindi il [[Secondo principio della dinamica|secondo principio della dinamica]]
$$
\vec{P}=m\vec{g}
$$
inoltre sappiamo che $m\vec{g}=-mg\hat{k}=m\ddot{y}k\implies\ddot{y}=-g$, allora risolvendo le [[Equazione differenziale|equazioni differenziali]] con $t_0=0,\dot{y}(t_0)=0,y(t_0)=h$ otteniamo che
$$
\dot{y}=\dot{y}_0+\int^t_0{-g}ds\implies\dot{y}=-gt
$$
$$
y=y_0+\int^t_0\dot{y}ds=h-\int^t_0-gsds=h-\frac12gt^2
$$
abbiamo quindi la seguente [[Equazione oraria|legge oraria]] $y(t)=h-\frac12gt^2$
* il tempo di caduta risulta essere $y(t_c)=0\implies t_c=\sqrt{\frac{2h}{g}}$
* la velocità massima è $v_M=|v(t_c)|=\sqrt{2gh}$ 

Notiamo infine che nel tempo di caduta non è presente il termine della massa, implicando che ogni corpo cade alla stessa velocità a meno di altre forze in gioco.
![[Moto dei gravi.excalidraw]]