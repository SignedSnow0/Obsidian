---
subject: fisica generale
type: definizione
---
Preso uno [[Spostamento|spostamento]] lungo una [[Traiettoria|traiettoria]] otteniamo la velocità vettoriale media tra i due estremi dello [[Spostamento|spostamento]] come il rapporto della distanza percorsa e il tempo impiegato
$$
\vec{v}_m(t,t+\Delta t)=\frac{\Delta\vec{r}}{\Delta t}=\frac{\vec{r}(t+\Delta t)-\vec{r}(t)}{\Delta t}
$$
Facendo tendere $\Delta t$ a $0$ otteniamo la formula della velocità vettoriale istantanea calcolata in un singolo punto
$$
\vec{v}=\lim_{\Delta t\to0}\vec{v}_m=\lim_{\Delta t\to0}\frac{\vec{r}(t+\Delta t)-\vec{r}(t)}{\Delta t}=\frac{d\vec{r}}{dt}=\dot{\vec{r}}
$$
Inoltre notiamo che nel limite $\Delta t\to0$ la direzione del vettore [[Spostamento|spostamento]] tende ad essere tangente alla [[Traiettoria|traiettoria]] nel punto valutato, perciò usando la [[Rappresentazione intrinseca|rappresentazione intrinseca]] e l'associata [[Velocità scalare|velocità scalare]] possiamo ricavare la [[Velocità vettoriale|velocità vettoriale]] come 
$$
\vec{v}=\dot{s}\hat{u}_t
$$
---
Vice versa, se abbiamo data l'[[Accelerazione vettoriale|accelerazione vettoriale]]
allora abbiamo un'[[Equazione differenziale|equazione differenziale]] tipo 
$$
\vec{v}(t)=\vec{a}(t)
$$
con infinite soluzioni possibili, ma data una velocità iniziale $\vec{v}(t_0)=\vec{v}_0$ in, allora il problema diventa un [[Problema di Cauchy|problema di Cauchy]]
$$
\begin{cases}\vec{v}(t)=\vec{a}(t)\\\vec{v}(t_0)=\vec{v}_0\end{cases}
$$
con soluzione 
$$
\vec{v}(t)=\vec{v}_0+\int_{t_0}^t\vec{a}(s)ds
$$