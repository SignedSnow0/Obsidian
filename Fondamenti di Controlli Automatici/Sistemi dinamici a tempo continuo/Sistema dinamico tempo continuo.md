> [!definition] Sistema dinamico tempo continuo
> Un sistema dinamico tempo continuo è rappresentato da un set di due equazioni:
> $$
> \frac{d\mathbf{x}}{dt}=f(\mathbf{x},\mathbf{u},t)
> $$
> $$
> \mathbf{y}=g(\mathbf{x},\mathbf{u},t)
> $$
> In entrambi i casi $\vec{x}$ indica lo stato attuale del sistema, $u$ rappresenta l'ingresso e $t$ il tempo.
> * L'[[Equazione differenziale|equazione differenziale]] dipendente dalla funzione $f$ indica l'evoluzione del sistema, chiamata **movimento dello stato**.
> * L'equazione algebrica dipendente dalla funzione $g$ rappresenta l'uscita del sistema, chiamata **movimento dell'uscita**.
---
### Classificazioni di sistemi dinamici tempo continui
A seconda di casi particolari delle funzioni nella definizione ($f$ e $g$) in input e output si hanno particolari sistemi dinamici, tra cui:
> [!definition] Sistemi monovariabili e multivariabili
> * Si dicono **sistemi monovariabili** (SISO) i sistemi dotati di una singola variabile di ingresso ed una singola variabile di uscita, cioè dove $\mathbf{u}=x\in\mathbb{R}$ e $\bf{y}=y\in\mathbb{R}$.
> * Si dicono invece **sistemi multivariabili** (MIMO) tutti gli altri sistemi.

> [!definition] Sistemi strettamente propri e non dinamici
> * Se la funzione di output non dipende dall'ingresso, cioè
> $$
> \mathbf{y}=g(\mathbf{x},t)
> $$
> allora il sistema si dice **strettamente proprio** o **puramente dinamico**.
> * Se invece l'uscita dipende solo dall'ingresso il sistema si dice **non dinamico** o **statico**, allora si ha
> $$
> \mathbf{y}=(\mathbf{u},t)
> $$

> [!definition] Sistemi tempo varianti e invarianti
> * Se le funzioni di stato e uscita non dipendono direttamente dal tempo, cioè
> $$
> \frac{d\mathbf{x}}{dt}=f(\mathbf{x},\mathbf{u})
> $$
> $$
> \mathbf{y}=g(\mathbf{x},\mathbf{u})
> $$
> allora il sistema si dice **tempo invariante**.
> * Altrimenti il sistema si dice **tempo variante**.

> [!definition] Sistemi lineari e non lineari
> * Se $f$ e $g$ sono lineari in $\mathbf{x}$ e $\mathbf{u}$, allora 
> $$
> \frac{d\mathbf{x}}{dt}=\mathbf{A}\mathbf{x}+\mathbf{B}\mathbf{u}
> $$
> $$
> \mathbf{y}=\mathbf{C}\mathbf{x}+\mathbf{D}\mathbf{u}
> $$
> allora il sistema si dice **lineare**.
> * Altrimenti il sistema si dice **non lineare**