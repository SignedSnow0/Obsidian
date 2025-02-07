## Classico
Il metodo classico consiste nell'elencare tutte le forze del sistema per poi sommarle, e usando il [[Secondo principio della dinamica|secondo principio della dinamica]], trovare la [[Equazione oraria|legge oraria]].
Elenchiamo quindi le forze in gioco:
1. Gravitazionale $\vec{g}=mg$
2. Tensione ([[Vincolo|vincolo]]) $\vec{T}$, dato che $\vec{T}\perp\hat{u}_t$ si ha che $\vec{T}$ non influisce nel moto del pendolo ($\vec{T}\cdot\vec{v}=0$), perciò può essere ignorato.

Allora l'unica forza nel sistema è [[La componente|la componente tangenziale]] di $\vec{g}$, cioè $mg\sin\theta$
Applicando il [[Secondo principio della dinamica|secondo principio della dinamica]] $\sum\vec{F}=m\vec{a}$ si ha 
$$
-mg\sin\theta=m\ddot{s}\implies \ddot{s}=-g\sin\theta
$$
dato che $\ddot{s}=l\ddot\theta$
$$
\ddot\theta=-\frac{g}{l}\sin\theta
$$
## Lagrange
Il metodo di Lagrange consiste nel trovare l'energia cinetica $K$ e l'energia potenziale $U$ e trovare quindi la lagrangiana
$$
\mathcal{L}=K-U
$$
Nel caso del pendolo l'energia cinetica è
$$
K=\frac12m\dot{s}^2=\frac12ml^2\dot\theta^2
$$
e l'energia potenziale è (scelto $y=0$ come perno del pendolo)
$$
U=mgy=-mgl\cos\theta
$$
quindi 
$$
\mathcal{L}=\frac12ml^2\dot\theta^2+mgl\cos\theta
$$
a questo punto scriviamo l'equazione di Eulero-Lagrange derivata dal principio di minima azione
$$
\frac{d}{dt}\frac{\partial\mathcal{L}}{\partial\dot\theta}=\frac{\partial\mathcal{L}}{\partial\theta}
$$
quindi
$$
\frac{\partial\mathcal{L}}{\partial\theta}=-mgl\sin\theta
$$
$$
\frac{\partial\mathcal{L}}{\partial\dot\theta}=ml^2\dot\theta
$$
$$
\frac{d}{dt}\frac{\partial\mathcal{L}}{\partial\dot\theta}=ml^2\ddot\theta
$$
$$
ml^2\ddot\theta=-mgl\sin\theta\implies\ddot\theta=-\frac{g}{l}\theta
$$
tornano all'equazione del metodo classico.
## Hamilton
Procediamo in maniera simile al metodo di Lagrange, ma invece di trovare la lagrangiana, troviamo l'energia totale**!!** o hamiltoniana
$$
E=K+U=\frac12ml^2\dot\theta^2-mgl\cos\theta
$$
Riscrivendo l'equazione in termini di momento $P=m\dot{s}=ml^2\dot\theta$ troviamo l'hamiltoniana
$$
\mathcal{H}=E=\frac{P^2}{2ml^2}-mgl\cos\theta
$$
risolviamo ora le equazioni di Hamilton
$$
\begin{cases}\displaystyle\dot{\theta}=\frac{\partial\mathcal{H}}{\partial P}\\\displaystyle\dot{P}=-\frac{\partial\cal{H}}{\partial\theta}\end{cases}
$$
nel nostro caso
$$
\begin{cases}\displaystyle\dot{\theta}=\frac{P}{ml^2}\\\displaystyle\dot{P}=-mgl\sin\theta\end{cases}
$$
$$
\begin{cases}\displaystyle ml^2\dot{\theta}=P\\\displaystyle\dot{P}=-mgl\sin\theta\end{cases}
$$
$$
\begin{cases}\displaystyle ml^2\ddot{\theta}=\dot{P}\\\displaystyle\dot{P}=-mgl\sin\theta\end{cases}
$$
$$
ml^2\ddot{\theta}=-mgl\sin\theta\implies\ddot\theta=-\frac{g}{l}\sin\theta
$$
