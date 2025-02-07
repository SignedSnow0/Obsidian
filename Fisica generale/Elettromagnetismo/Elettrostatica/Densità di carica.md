---
subject: fisica generale
type: definizione
---
Per praticità nel calcolo di sistemi di [[Carica elettrica|cariche]], nonostante esse siano oggetti quantizzati, vengono spesso descritte come una distribuzione continua del loro valore medio su un determinato volume.
### Densità lineare
Per calcolare la densità su una superficie di una dimensione si fa il rapporto incrementale tra una funzione che descrive la quantità di carica $q$ e lo spostamento $l$ lungo l'[[Rappresentazione intrinseca|ascissa curvilinea]]
$$
\lambda=\lim_{\Delta l\to0}\frac{\Delta q}{\Delta l}=\frac{dq}{dl}
$$
perciò la carica totale è 
$$
q_l=\int_l\lambda dl
$$
e ricordano la costruzione del [[Campo elettrostatico|campo elettrostatico]]
$$
\vec{E}(\vec{r})=\frac{1}{4\pi\epsilon_0}\int\frac{\lambda(\vec{r}_\lambda)(\vec{r}-\vec{r}_\lambda)}{|\vec{r}-\vec{r}_\lambda|^3}dl
$$
### Densità superficiale
Per calcolare la densità superficiale si ragiona in maniera analoga alla densità lineare prendendo in considerazione però una differenza di area $S$
$$
\sigma=\lim_{\Delta S\to0}\frac{\Delta q}{\Delta S}=\frac{dq}{dS}
$$
la carica totale è quindi
$$
q_S=\iint_S\sigma ds
$$
e ricordano la costruzione del [[Campo elettrostatico|campo elettrostatico]]
$$
\vec{E}(\vec{r})=\frac{1}{4\pi\epsilon_0}\iint_S\frac{\sigma(\vec{r}_\sigma)(\vec{r}-\vec{r}_\sigma)}{|\vec{r}-\vec{r}_\sigma|^3}dS
$$
### Densità volumetrica
Ancora un altra volta si ragiona in maniera analoga considerando però una differenza di volume $V$
$$
\rho=\lim_{\Delta V\to0}\frac{\Delta q}{\Delta V}=\frac{d q}{dV}
$$
di conseguenza la carica totale è 
$$
q_V=\iiint_V\rho dV
$$
e ricordano la costruzione del [[Campo elettrostatico|campo elettrostatico]]
$$
\vec{E}(\vec{r})=\frac{1}{4\pi\epsilon_0}\iiint_V\frac{\rho(\vec{r}_\rho)(\vec{r}-\vec{r}_\rho)}{|\vec{r}-\vec{r}_\rho|^3}dV
$$
![[Densita di carica.excalidraw]]