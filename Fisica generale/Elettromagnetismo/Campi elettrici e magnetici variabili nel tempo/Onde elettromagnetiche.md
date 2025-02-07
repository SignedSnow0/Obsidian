---
subject: fisica generale
type: definizione
---
Prendendo in considerazione le [[Equazioni di Maxwell|equazioni di Maxwell]] in assenza cariche si ha
$$
\vec\nabla\cdot\vec{E}=0\quad\quad\vec\nabla\cdot\vec{B}=0
$$
$$
\vec\nabla\wedge\vec{E}=-\frac{\partial\vec{B}}{\partial t}\quad\quad\vec\nabla\wedge\vec{B}=\mu_0\epsilon_0\frac{\partial\vec{E}}{\partial t}
$$
mettendo in relazione queste quattro leggi si ottiene che le onde elettromagnetiche sono descritte da due equazioni d'onda attraverso il campo elettromagnetico
$$
\square\vec{E}=0\quad\quad\square\vec{B}=0
$$
con $\displaystyle\mu_0\epsilon_0=\frac{1}{c^2}$ e $\displaystyle c=3\times10^{8}\ \frac{m}{s}$

---
Applicando il rotore alla [[Equazioni di Maxwell|seconda legge di Maxwell]] si ha
$$
\vec\nabla\wedge\left(\vec\nabla\wedge\vec{E}\right)=\vec\nabla\wedge\left(-\frac{\partial\vec{B}}{\partial t}\right)=-\frac{\partial}{\partial t}\left(\vec\nabla\wedge\vec{B}\right)
$$
dalla [[Equazioni di Maxwell|quarta legge di Maxwell]] si ha
$$
\vec\nabla\wedge\vec{B}=\mu_0\epsilon_0\frac{\partial\vec{E}}{\partial t}\implies-\frac{\partial}{\partial t}\left(\vec\nabla\wedge\vec{B}\right)=-\mu_0\epsilon_0\frac{\partial^2\vec{E}}{\partial t^2}
$$
invece dall'identità vettoriale del rotore di rotore si ha
$$
\vec\nabla\wedge\left(\vec\nabla\wedge\vec{E}\right)=-\vec\nabla^2\vec{E}+\vec\nabla(\vec\nabla\cdot\vec{E})
$$
dalla [[Equazioni di Maxwell|prima legge di Maxwell]] si ha
$$
\vec\nabla\cdot\vec{E}=0\implies-\nabla^2\vec{E}+\vec\nabla(\vec\nabla\cdot\vec{E})=-\nabla^2\vec{E}
$$
perciò ricombinando all'equazione inziale si ha
$$
\nabla^2\vec{E}=\mu_0\epsilon_0\frac{\partial^2\vec{E}}{\partial t^2}
$$
ponendo $\displaystyle\mu_0\epsilon_0=\frac{1}{c^2}$ si ha
$$
\square\vec{E}=0
$$