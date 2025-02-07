---
subject: fisica generale
type: definizione
---
Il lavoro è la capacità di una [[Secondo principio della dinamica|forza]] di compiere uno [[Spostamento|spostamento]].
Dato un [[Punto materiale|punto materiale]] che si sposta lungo una [[Traiettoria|curva]] $l$ e una forza $\vec{F}$ che agisce sul punto, definiamo il lavoro infinitesimo come lo spostamento della forza parallela alla curva in un tratto infinitesimo di essa
$$
\delta L=\vec{F}\cdot d\vec{l}
$$
avremo allora che il lavoro totale sul percorso tra $A$ e $B$ è la somma di tutti gli infinitesimi, cioè
$$
L=\int_A^B\vec{F}\cdot d\vec{l}
$$
l'[[Unità di misura|unità di misura]] del lavoro è il *Joule* $J=N\cdot m$
$$
[L]=[ML^2T^{-2}]
$$
Se il lavoro è compiuto per un campo [[Campo delle forze conservative|conservativo]], allora il lavoro sarà uguale alla differenza di [[Energia potenziale|energia potenziale]]
$$
L_{A,B}=U(A)-U(B)
$$
se invece il campo non è [[Campo vettoriale conservativo|conservativo]] il lavoro è dato dal teorema delle forze vive
$$
L_{A,B}=K(B)-K(A)
$$
dove questo tipo di lavoro è distinguibile nella parte svolta dalle forze conservative e non
$$
L_{A,B}=L_{cons}+L_{nc}
$$
allora si ha che il lavoro disperso è la differenza di energia meccanica totale
$$
L_{nc}=[T(B)+U(B)]-[T(A)+U(A)]=E(B)-E(A)
$$
---
Notiamo che se la forza è parallela allo spostamento si ha
$$
L=\int_A^B\vec{F}\cdot d\vec{l}=\int_A^B|\vec{F}|\cos(0)d|\vec{l}|=\int_A^BFdl=F\int_A^Bdl=Fl
$$
se invece l'angolo è costante si ha
$$
L=\int_A^B\vec{F}\cdot d\vec{l}=\int_A^B|\vec{F}|\cos\theta d|\vec{l}|=\int_A^BF\cos\theta dl=F\cos\theta\int_A^Bdl=F\cos\theta l
$$