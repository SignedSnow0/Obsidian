---
subject: fisica generale
type: definizione
---
Il modello di Drude-Lorentz descrive il comportamento degli elettroni liberi in analogia con il comportamento di molecole di gas attraverso un reticolo cristallino.
Sperimentalmente si osserva che la velocità media degli elettroni è proporzionale al campo di cui sono soggetti
$$
\langle\vec{v}_e\rangle\propto\vec{E}
$$
per il [[Secondo principio della dinamica|secondo principio della dinamica]] si ha che 
$$
\vec{a}_e=\frac{\vec{F}_e}{m_e}=\frac{q_e}{m_e}\vec{E}
$$
Prendiamo ora in considerazione il reticolo di atomi, e definiamo come $p(t)$ la [[Funzione densità|probabilità]] di avere un urto in un istante $t$, allora il [[Valore atteso|tempo medio]] fra due urti sarà
$$
\langle t\rangle=\int_0^\infty tp(t)dt
$$
dato che nel tempo fra due urti la velocità aumenterà linearmente (moto uniformemente accelerato) la velocità è
$$
\vec{v}_e=\frac{q_e}{m_e}\vec{E}t
$$
perciò la [[Valore atteso|velocità media]] sarà
$$
\langle\vec{v}_e\rangle=\int_0^\infty \vec{v}_e(t)p(t)dt=\int_0^\infty dt\frac{q_e}{m_e}\vec{E}tp(t)=\frac{q_e}{m_e}\vec{E}\langle t\rangle
$$
che viene chiamata velocità di deriva
$$
\vec{v}_d=\langle\vec{v}_e\rangle=\frac{q_e}{m_e}\vec{E}\langle t\rangle
$$
che è proporzionale al campo, ha stessa direzione e verso opposto.