---
subject: fisica generale
type: definizione
---
La legge di Ampère mette in relazione la circuitazione di un il campo magnetico con le correnti concatenate
$$
\oint_\Gamma\vec{B}\cdot d\vec{l}=\mu_0\sum_k^{\text{conc}}i_k
$$
Usando il [[Formula di Stokes|teorema di Stokes]] si ha che
$$
\oint_\Gamma\vec{B}\cdot d\vec{l}=\iint_{S_\Gamma}\vec\nabla\wedge\vec{B}\cdot d\hat{S}
$$
riscrivendo la somma di correnti in termini di [[Densità di corrente|densità di corrente]]
$$
\sum i_k=\sum\iint\vec{J}_k\cdot d\hat{S}=\iint\vec{J}_c\cdot d\hat{S}
$$
unendo i due si ha
$$
\iint\vec\nabla\wedge\vec{B}\cdot d\hat{S}=\mu_0\iint\vec{J}_c\cdot d\hat{S}
$$
ottenendo la legge di Ampère in forma locale
$$
\vec\nabla\wedge\vec{B}=\mu_0\vec{J}
$$
---
Prendiamo in considerazione una circuitazione che concatena un filo attraversato da [[Intensità di corrente|corrente]], dalla [[Legge di Biot-Savart|legge di Biot-Savart]] sappiamo che
$$
\vec{B}\cdot d\vec{l}=\frac{\mu_0i}{2\pi r}\hat{u}_t\cdot d\vec{l}=\frac{\mu_0i}{2\pi}d\theta
$$
allora considerando il campo su tutta la circuitazione si ha
$$
\oint_\Gamma\vec{B}\cdot d\vec{l}=\int_0^{2\pi}\frac{\mu_0i}{2\pi}d\theta=\pm\mu_0i
$$
secondo la regola della mano destra.
Se invece la circuitazione non concatena il filo si avrà che per ogni $d\theta$ ci saranno due tratti di verso opposto che si annullano
$$
\oint\vec{B}\cdot d\vec{l}=0
$$
allora unendo i due casi si ottiene la legge di Ampère
$$
\oint_\Gamma\vec{B}\cdot d\vec{l}=\mu_0\sum_k^{\text{conc}}i_k
$$