> [!definition] Equilibrio di un sistema
> Dato un [[Sistema dinamico tempo continuo|sistema dinamico]] sottoposto a ingresso costante $\bf{u}=\bar{\bf{u}}$ allora il sistema è detto in equilibrio se il movimento del sistema $\dot{\bf{x}}$ è nullo, cioè 
> $$
> f(\bar{\bf{x}},\bar{\bf{u}})=\bf{0}
> $$
> dove $\bar{\bf{x}}$ sono i possibili andamenti che soddisfano la condizione di equilibrio.
> Allora dato che lo stato del sistema $\bar{\bf{x}}$ è costante l'uscita altrettanto costante e pari a 
> $$
> \bar{\bf{y}}=g(\bar{\bf{x}},\bar{\bf{u}})
> $$

> [!definition] Stabilità
> Il concetto di stabilità indica la capacità di un sistema di rimanere in uno stato di equilibrio $\bar{\bf{x}}$ partendo da uno stato iniziale $\bf{x}_0$ a fronte di una variazione di esso, in termini matematici un sistema tempo invariante è stabile se
> $$
> \forall\epsilon>0\quad\exists\delta>0:\quad||\bf{x}_0-\bar{\bf{x}}||\le\delta\implies||\bf{x}-\bar{\bf{x}}||\le\epsilon
> $$
> inoltre uno stato di equilibrio si dice asintoticamente stabile se inoltre 
> $$
> \lim_{t\to+\infty}||\bf{x}-\bar{\bf{x}}||=0
> $$
> ---
> Inoltre la stabilità può essere una proprietà del'equilibrio dello stato con definizioni analoghe.