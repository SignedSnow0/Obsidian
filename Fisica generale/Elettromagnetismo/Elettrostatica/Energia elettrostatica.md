---
subject: fisica generale
type: definizione
---
Dalla [[Legge di Coulomb|legge di Coulomb]] sappiamo che la forza elettrostatica è proporzionale al [[Campo elettrostatico|campo elettrostatico]]
$$
\vec{F}_{\text{el}}=q\vec{E}
$$
inoltre se il [[Campo elettrostatico|campo]] è [[Campo vettoriale conservativo|conservativo]] sappiamo che possiede un [[Potenziale elettrostatico|potenziale]], quindi con questi due fatti otteniamo che
$$
\mathcal{L}_{\text{el}}=\int_A^B\vec{F}_{\text{el}}\cdot d\vec{l}=\int_A^Bq\vec{E}\cdot d\vec{l}=q\int_A^B\vec{E}\cdot d\vec{l}=q(V_A-V_B)=q\Delta V_{AB}
$$
Allora definiamo l'energia potenziale di una [[Carica elettrica|carica]] come
$$
U_e=qV
$$
dove $U$ è misurate in Joule o in elettronvolt
$$
1eV=q_e\Delta V=1.6\times10^{-19}J
$$
Infine, dato che forza elettrostatica è conservativa l'energia meccanica è una quantità conservata
$$
\mathcal{E}=K+U_e
$$
e la variazione di energia potenziale corrisponde a una variazione di energia cinetica
$$
K_1+U_1=K_2+U_2
$$
---
In un sistema di $n$ cariche l'energia elettrostatica è definita come il lavoro necessario per portare un ulteriore carica nel sistema, per il principio di sovrapposizione l'energia totale è la somma delle singole energie fra le $n$ cariche
$$
U_e=U_{12}+\dots+U_{ij}
$$
per semplicità di calcolo è utile calcolare tutte le permutazioni con ripetizione e dividere per $2$
$$
U_e=\frac12\sum q_iV_i=\sum_{i=1}\sum_{j=1,\ j\ne i}\frac{q_iq_j}{4\pi\epsilon_0 r_{ij}}
$$
