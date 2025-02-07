---
subject: fisica generale
type: definizione
---
Dal [[Modello di Drude-Lorentz|modello di Drude-Lorentz]] di corrente si ha che
$$
\vec{v}_d=\frac{q_e}{m_e}\vec{E}
$$
moltiplicando la velocità di deriva per il numero di portatori di carica e la carica fondamentale dell'elettrone
si ha
$$
nq_e\vec{v}_d=\frac{nq_e^2}{m_e}\langle t\rangle\vec{E}
$$
ricordando ora la definizione di [[Densità di corrente|densità di corrente]] si ha 
$$
\vec{J}=\left[\frac{nq_e^2}{m_e}\langle t\rangle\right]\vec{E}
$$
raccogliamo il termine tra parentesi e lo chiamiamo conduttività elettrica
$$
\sigma_C=\frac{nq_e^2}{m_e}\langle t\rangle
$$
e definiamo il suo inverso come resistività elettrica
$$
\rho_R=\frac{1}{\sigma_C}
$$
allora otteniamo la legge di Ohm in forma locale
* $$
\vec{J}=\sigma_C\vec{E}
$$
* $$
\vec{E}=\rho_R\vec{J}
$$
---
Considerando invece un conduttore ricordiamo che
$$
|\Delta V|=\int\vec{E}\cdot d\vec{l}=El
$$
allora 
$$
El=\rho_Rjl=\rho_Rjl\frac{S}{S}
$$
dove $S$ è la sezione del conduttore, quindi
$$
El=\left[\rho_R\frac{l}{S}\right]jS=\left[\rho_R\frac{l}{S}\right]i
$$
definendo $R$ si ottiene la seconda legge di Ohm
$$
R=\rho_R\frac{l}{S}
$$
e quindi segue la prima legge di Ohm
$$
\Delta V=Ri
$$