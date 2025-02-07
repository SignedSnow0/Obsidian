---
subject: analisi 2
type: dimostrazione
---
Sia $I\subseteq\mathbb{R}$ aperto e non vuoto, $a_0,\dots,a_{m-1}\in\mathcal{C}(I)$, 
$$
T:\mathcal{C}^m(I)\to\mathcal{C}(I),\quad Tx=x^{(m)}-a_0x-\dots-a_{m-1}x^{(m-1)}
$$
allora $T$ è una [[Applicazione lineare|applicazione lineare]] tra gli [[Spazio vettoriale|spazi vettoriali]] $\mathcal{C}^m(I)$ e $\mathcal{C}^m(I)$
# Dimostrazione
Sia $x,y\in\mathcal{C}^m(I),\lambda,\mu\in\mathbb{R}$, allora
$$
T(\lambda x+\mu y)=(\lambda x+\mu y)^{(m)}-a_0(\lambda x+\mu y)-\dots-a_{m-1}(\lambda x+\mu y)^{(m-1)}=
$$
$$
\lambda x^{(m)}+\mu y^{(m)}-a_0\lambda x-a_0\mu y-\dots-a_{m-1}(\lambda x^{(m-1)}+\mu y^{(m-1)})=
$$
$$
\lambda(x^{(m)}-a_0x-\dots-a_{m-1}x^{(m-1)})+\mu(x^{(m)}-a_0x-\dots-a_{m-1}x^{(m-1)})=
$$
$$
\lambda Tx+\mu Ty\quad\square
$$