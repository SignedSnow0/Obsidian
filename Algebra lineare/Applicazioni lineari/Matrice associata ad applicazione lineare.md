---
subject: algebra lineare
type: definizione
---
Sia $f:V\to W$ un'[[Applicazione lineare|applicazione lineare]] e $V,W$ [[Spazio vettoriale|spazi vettoriali]] con $\dim V=n,\dim W=m$ e $\mathcal{B}=\{v_1,\dots,v_n\},\mathcal{B}'=\{w_1,\dots,w_m\}$ due [[Base|basi]] per $V$ e $W$, se ogni $v_j$ è rappresentabile come [[Combinazione lineare|combinazione lineare]] di $\mathcal{B}'$ allora esiste una  matrice $M_{\mathcal{B},\mathcal{B}'}(f)=(a_{ij})$ tale che $\forall v\in V\quad f(v)\in W$ ha coordinate rispetto $\mathcal{B}'$ tali che
$$
\begin{pmatrix}c_1\\\vdots\\c_m\end{pmatrix}_{\mathcal{B}'}=M_{\mathcal{B},\mathcal{B}'}(f)\begin{pmatrix}b_1\\\vdots\\b_n\end{pmatrix}_{\mathcal{B}}
$$
dove $b_j$ sono le coordinate di $v$ rispetto a $\mathcal{B}$.