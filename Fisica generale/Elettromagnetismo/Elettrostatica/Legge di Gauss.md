---
subject: fisica generale
type: definizione
---
La legge di Gauss correla il [[Flusso|flusso]] del campo elettrico attraverso una [[Superficie orientata|superficie]] chiusa $S$ con le cariche contenute al suo interno con la seguente relazione:
$$
\Phi_S(\vec{E})=\oiint\vec{E}\cdot d\hat{S}=\frac{Q_{s}}{\epsilon_{0}}=\frac{1}{\epsilon_0}\iiint_{V_S}\rho dV
$$
Ricordando il [[Teorema della divergenza|teorema della divergenza]] si ha che
$$
\Phi_S(\vec{E})=\oiint_{S}\vec{E}\cdot\hat{n}dS=\iiint_{V_S}\vec{\nabla}\cdot\vec{E}dV=\frac{1}{\epsilon_0}\iiint\rho dV
$$
perciò derivando si ottiene la legge di Gauss in forma differenziale
$$
\vec{\nabla}\cdot\vec{E}=\frac{\rho}{\epsilon_0}
$$
dove $\rho$ è la [[Densità di carica|densità di carica]].
![[Flusso.excalidraw]]
---
Consideriamo il [[Flusso|flusso]] del campo elettrico di una [[Carica elettrica|carica]] interna attraverso una superficie chiusa:
attraverso una parte infinitesima si ha
$$
d\Phi_S(\vec{E})=\vec{E}\cdot d\hat{S}=EdS\cos\alpha=Ed\Sigma
$$
$E$ è il [[Campo elettrostatico|campo elettrostatico]] uguale a
$$
\frac{q}{4\pi\epsilon_0r^2}
$$
$d\Sigma$ è un infinitesimo di superficie attraversata dal flusso uguale a
$$
r^2d\Omega
$$
dove $\Omega$ è l'[[Angolo solido|angolo solido]]
allora il flusso totale è
$$
\Phi_S(\vec{E})=\oiint d\Phi_S(\vec{E})=\oiint\vec{E}\cdot d\hat{S}=\frac{q}{4\pi\epsilon_0}\oiint d\Omega=\frac{q}{\epsilon_0}
$$
Se invece la carica è esterna alla superficie si ha che per ogni linea di campo entrante alla superficie ne corrisponde una uscente che formano angoli complementari con il loro normale, perciò 
$$
\Phi_S(\vec{E})=0
$$
Perciò ora applicando il [[Principio di sovrapposizione|principio di sovrapposizione]] alle cariche si ottiene la legge di Gauss
$$
\Phi_S(\vec{E})=\oiint\vec{E}\cdot d\hat{S}=\frac{Q_s}{\epsilon_0}=\frac{1}{\epsilon_0}\iiint_{V_S}\rho dV
$$