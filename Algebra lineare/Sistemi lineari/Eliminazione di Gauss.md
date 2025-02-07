---
subject: algebra lineare
type: procedimento
---
Data una [[Matrice|matrice]] $A$ seguiamo questi passaggi per ottenere una matrice ridotta
1. Prendiamo la prima colonna non nulla di $A$ con indice $j_1$, allora prendiamo il primo elemento non nullo nella colonna $a_{i_1j_1}$, se $i_1=1$ si passa al punto 2, altrimenti si passa al punto 3
2. Scambiamo la riga contenente l'elemento cercato in 1 ($i_1$) con la prima riga
3. Eliminiamo nella $j_1$-esima colonna tutti gli elementi diversi da zero sotto la prima riga senza modificarne la prima
4. Ripetere i passaggi partendo dalla riga inferiore ogni  iterazione.
Allora otterremo una [[Matrice triangolare|matrice triangolare superiore]] dove ogni elemento sotto il primo non nullo di ogni riga è composto da soli zeri, cioè a gradini
$$
\begin{pmatrix}
0&\dots&0&p_1&\dots&\dots\\
\vdots&\vdots&\vdots&\vdots&\vdots&\vdots\\
0&\dots&\dots&\dots&0&p_n
\end{pmatrix}
$$
dove ogni elemento $p_j$ viene chiamato pivot.