---
subject: fisica generale
type: definizione
---
Per garantire il principio di località molti studi della fisica fanno usa di [[Campo vettoriale|campio vettoriali]], come il campo elettrostatico.
È possibile associare ad ogni punto dello spazio una forza generata dalla [[Legge di Coulomb|legge di Coulomb]] da una o più [[Carica elettrica|cariche]], andando così a formare un [[Campo vettoriale|campo vettoriale]] $\vec{E}$ con la seguente formula (per una singola carica di intensità $Q$) 
$$
\vec{E}(\vec{r})=\frac{1}{4\pi\epsilon_0}\frac{Q}{r^2}\hat{u}_r
$$
Se invece vogliamo descrivere la forza percepita da una particella $q$ nel campo usiamo la seguente formula
$$
\vec{F}(\vec{r})=q\vec{E}(\vec{r})
$$
Il campo elettrostatico è misurato in **newton/coulomb** o **volt/metro**
$$
[\vec{E}]=[FQ^{-1}]=[MLT^{-3}I^{-1}]
$$
---
Inoltre il campo elettrostatico ha le seguenti proprietà:
1. Il [[Campo vettoriale|campo]] è [[Campo vettoriale conservativo|conservativo]]
$$
\oint\vec{E}\cdot d\vec{l}=0
$$
2. Il [[Campo vettoriale|campo vettoriale]] è irrotazionale
$$
\vec{\nabla}\wedge\vec{E}=0
$$
3. Il campo è [[Campo vettoriale esatto|esatto]] 
$$
\vec{E}=-\vec{\nabla}V
$$
dove $V$ è chiamato [[Potenziale elettrostatico|potenziale elettrico]]
4. Dalla definizione di [[Potenziale|potenziale]] e dalla 3 si ha 
$$
\int_A^B\vec{E}\cdot d\vec{l}=V(A)-V(B)
$$
5. Dal [[Principio di sovrapposizione|principio di sovrapposizione]] della [[Legge di Coulomb|forza di Coulomb]] abbiamo che se nel campo agiscono più cariche risulta
$$ 
\vec{E}=\sum_i\vec{E}_i
$$
![[Campo elettrostatico.excalidraw]]