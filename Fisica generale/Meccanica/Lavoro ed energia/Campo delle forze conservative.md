---
subject: fisica generale
type: definizione
---
Se il [[Lavoro|lavoro]] compiuto da una forza non dipende dalla traiettoria si dice che la forza è conservativa, i [[Campo vettoriale|campi]] descritti da queste forze hanno diverse proprietà utili:
1. Per definizione il [[Campo vettoriale|campo]] è [[Campo vettoriale conservativo|conservativo]], quindi
$$
L_{A,A}=\oint\vec{F}\cdot d\vec{l}=0
$$
2. Per la proprietà 1, il [[Campo vettoriale|campo]] è irrotazionale, cioè
$$
\vec{\nabla}\wedge\vec{F}=0
$$
3. Dalla prima o seconda proprietà ricaviamo che il [[Campo vettoriale|campo]] è [[Campo vettoriale esatto|esatto]], esiste quindi **almeno** un [[Potenziale|potenziale]] $U$, chiamato [[Energia potenziale|energia potenziale]], con il quale possiamo descrivere il campo, per convenzione si usa 
$$
\vec{F}=-\vec{\nabla}U
$$
4. Dalle proprietà 1 e 3 si ha
$$
L_{A,B}=U(A)-U(B)
$$
---
Dal punto di vista fisico il [[Campo|campo]] si dice [[Campo vettoriale conservativo|conservativo]] perchè esiste una quantità che viene conservata, cioè non varia nel tempo: l'energia meccanica
$$
E=K+U
$$
Dal [[Teorema delle forze vive|teorema delle forze vive]] abbiamo che
$$
L_{A,B}=K(B)-K(A)
$$
inoltre dalla proprietà 4
$$
L_{A,B}=U(A)-U(B)
$$
perciò
$$
K(B)-K(A)=U(A)-U(B)\implies K(B)+U(B)=K(A)+U(A)\quad\square
$$