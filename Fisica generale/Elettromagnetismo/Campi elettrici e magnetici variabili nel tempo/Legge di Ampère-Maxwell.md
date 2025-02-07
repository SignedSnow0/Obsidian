---
subject: fisica generale
type: definizione
---
La legge di Ampère-Maxwell è una estensione della [[Legge di Ampère|legge di Ampère]] per [[Campo elettrostatico|campi elettrici]] variabili nel tempo.
$$
\vec\nabla\wedge\vec{B}=\mu_0\left(\vec{J}+\epsilon_0\frac{\partial\vec{E}}{\partial t}\right)
$$
* $\vec{J}$ è detta [[Densità di corrente|densità di corrente]] di conduzione, dovuta al moto delle cariche $\vec{J}_C$.
* $\epsilon_0\frac{\partial\vec{E}}{\partial t}$ è detta [[Densità di corrente|densità di corrente]] di spostamento, dovuta alla variazione del campo elettrico $\vec{J}_S$.

Questa legge mette in relazione il campo elettrico e magnetico, suggerendo che i due siano il risultato di una stessa forza comune.

A partire dalla [[Densità di corrente|densità di corrente]] di spostamento possiamo definire l'[[Intensità di corrente|intensità di corrente]] di spostamento:
$$
i_S=\iint\vec{J}_S d\hat{S}=\iint\epsilon_0\frac{\partial\vec{E}}{\partial t}\cdot d\hat{S}=\epsilon_0\frac{d}{dt}\iint\vec{E}\cdot d\hat{S}=\epsilon_0\frac{d\Phi_S(\vec{E})}{dt}
$$
arrivando quindi alla legge di Ampère-Maxwell in forma integrale
$$
\oint_\Gamma\vec{B}\cdot d\vec{l}=\mu_0\sum_k^{\text{conc}}(i_C+i_S)
$$
---
La [[Legge di Ampère|legge di Ampère]] presenta limitazioni per [[Campo elettrostatico|campi elettrici]] variabili nel tempo:
$$
\vec\nabla\wedge\vec{B}=\mu_0\vec{J}
$$
applichiamo ora l'operatore divergenza
$$
\vec\nabla\cdot\left(\vec\nabla\wedge\vec{B}\right)=\mu_0\vec\nabla\cdot\vec{J}
$$
allora si dimostra che 
$$
\vec\nabla\cdot\vec\nabla\wedge\vec{B}=0
$$
ma 
$$
\vec\nabla\cdot\vec{J}
$$
non è necessariamente $0$, portando a una contraddizione.
Ricordiamo ora l'[[Equazione di continuità|equazione di continuità]]
$$
\vec\nabla\cdot\vec{J}+\frac{\partial\rho}{\partial t}=0
$$
se la [[Densità di carica|densità di carica]] è costante nel tempo la sua derivata sarà nulla e quindi $\vec\nabla\cdot\vec{J}=0$ validando la classica [[Legge di Ampère|legge di Ampère]], altrimenti dalla [[Legge di Gauss|legge di Gauss]] si ha 
$$
\vec\nabla\cdot\vec{E}=\frac{\rho}{\epsilon_0}\implies\rho=\epsilon_0\vec\nabla\cdot\vec{E}
$$
allora
$$
\vec\nabla\cdot\vec{J}+\frac{\partial}{\partial t}(\epsilon_0\vec\nabla\cdot\vec{E})=0
$$
$$
\vec\nabla\cdot\left(\vec{J}+\epsilon_0\frac{\partial\vec{E}}{\partial t}\right)=0
$$
otteniamo quindi che questo vettore ha sempre divergenza nulla sia in presenza di correnti che non, arrivando quindi alla legge di Ampère-Maxwell
$$
\vec\nabla\wedge\vec{B}=\mu_0\left(\vec{J}+\epsilon_0\frac{\partial\vec{E}}{\partial t}\right)
$$