---
subject: fisica generale
type: definizione
---
Immaginiamo di avere un sistema di riferimento con centro $O$, allora per definizione il centro è stazionario, e ogni punto $P$ nello spazio è definito da
$$
\vec{r}=x\hat{i}+y\hat{j}+y\hat{k}
$$
se aggiungiamo un altro sistema di riferimento $O'$ mobile rispetto ad $O$ al variare del tempo, si avrà che
$$
\vec{r}=\vec{r}'+\vec{r}_{O'}
$$
dove $\vec{r}'$ è lo [[Spostamento|spostamento]] tra $O'$ e $P$, e $\vec{r}_{O'}$ è lo [[Spostamento|spostamento]] tra $O$ e $O'$
allora otteniamo la [[Velocità vettoriale|velocità]] relativa attraverso la sua definizione
$$
\vec{v}=\frac{d\vec{r}}{dt}=\frac{d\vec{r}'}{dt}+\frac{d\vec{r}_{O'}}{dt}
$$
il vettore $\displaystyle\frac{d\vec{r}_{O'}}{dt}$ è semplicemente la velocità rispetto a $O$, quindi $\vec{v}_{O'}$, invece $\displaystyle\frac{d\vec{r}'}{dt}$ dipende da un sistema di riferimento che è esso stesso in movimento, in generale risulta essere
$$
\frac{d\vec{r}'}{dt}=\vec{v}'+\vec{\omega}\times\vec{r}'
$$
dove $\vec{r}'$ è lo spostamento di $P$ da $O'$ e $\vec{\omega}$ è la [[Velocità vettoriale|velocità angolare]] del nuovo sistema di riferimento $O'$, e $\vec{v}'$ è la velocità di $P$ rispetto a $O'$, perciò
$$
\vec{v}=\vec{v}'+\vec\omega\times\vec{r}+\vec{v}_{O'}
$$
a volte l'equazione usa la seguente formulazione
$$
\vec{v}=\vec{v}'+\vec{v}_{\tau}
$$
con $\vec{v}_{\tau}$ che viene chiamata **velocità di trascinamento**.
In maniera analoga alla [[Velocità vettoriale|velocità]] si può derivare l'[[Accelerazione vettoriale|accelerazione]]
$$
\vec{a}=\vec{a}'+2\vec\omega\times\vec{v}'+\dot{\vec\omega}\times\vec{r}'+\vec\omega\times(\vec\omega\times\vec{r}')+\vec{a}_{O'}
$$
ponendo $\vec{a}_\tau=\dot{\vec\omega}\times\vec{r}'+\vec{\omega}\times(\vec{\omega}\times\vec{r}')+\vec{a}_{O'}$ e $\vec{a}_{\text{co}}=2\vec\omega\times\vec{v}'$ si ha
$$
\vec{a}=\vec{a}+\vec{a}_{\text{co}}+\vec{a}_{\tau}
$$