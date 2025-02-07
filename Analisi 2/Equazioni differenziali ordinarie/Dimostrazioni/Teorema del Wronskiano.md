---
subject: analisi 2
type: dimostrazione
---
Consideriamo l'[[ODE lineare|equazione lineare]] omogenea
$$
x^{(m)}(t)=a_0(t)x(t)+\dots+a_{m-1}(t)x^{(m-1)}(t)
$$
dove $I\subseteq\mathbb{R}$ non vuoto, siano $\psi_0,\dots,\psi_{m-1}$ una [[Soluzione massimale|soluzione lineare]], allora sono equivalenti:
1. $\{\psi_0,\dots,\psi_{m-1}\}$ è un [[Sistema fondamentale di soluzioni|sistema fondamentale di soluzioni]]
2. $\forall t\in I\quad w(\psi_0,\dots,\psi_{m-1})(t)\ne0$
3. $\exists t_0\in I:w(\psi_0,\dots,\psi_{m-1})(t_0)\ne 0$
# Dimostrazione
Verifichiamo che 1 implichi 2:
Sia $\{\psi_0,\dots,\psi_{m-1}\}$ [[Sistema fondamentale di soluzioni]] e supponiamo per assurdo che 
$$
\exists t_1\in I:w(\psi_0,\dots,\psi_{m-1})(t_1)=0
$$
allora le colonne del [[Wronskiano]]
$$
\begin{pmatrix}\psi_0(t_1)\\\vdots\\\psi_0^{(m-1)}(t_1)\end{pmatrix},\dots,\begin{pmatrix}\psi_{m-1}(t_1)\\\vdots\\\psi_{m-1}^{(m-1)}(t_1)\end{pmatrix}
$$
sono linearmente indipendenti, perciò esistono $c_0,\dots,c_{m-1}$ tali che
$$
c_0\psi_0(t_1)+\dots+c_{m-1}\psi_{m-1}(t_1)=0
$$
$$
\vdots
$$
$$
c_0\psi_0^{(m-1)}(t_1)+\dots+c_{m-1}\psi_{m-1}^{(m-1)}(t_1)=0
$$
consideriamo la funzione $\psi=c_0\psi_0+\dots+c_{m-1}\psi_{m-1}$, essa è soluzione dell'equazione differenziale e si annulla in $t_1$, allora per unicità della soluzione massimale $\psi(t)=0\quad\forall t\in I$ che contraddice il fatto che sia combinazione lineare di un [[Sistema fondamentale di soluzioni]].
Verifichiamo che 3 implichi 1:
Sia $c_0,\dots,c_{m-1}\in\mathbb{R}:$
$$
c_0\psi_0(t)+\dots+c_{m-1}\psi_{m-1}(t)=0\quad\forall t\in I
$$
allora
$$
c_0\psi_0'(t)+\dots+c_{m-1}\psi_{m-1}'(t)=0
$$
$$
\vdots
$$
$$
c_0\psi_0^{(m-1)}(t)+\dots+c_{m-1}\psi_{m-1}^{(m-1)}(t)=0
$$
In particolare se $t=t_0$
$$
c_0\psi_0'(t_0)+\dots+c_{m-1}\psi_{m-1}'(t_0)=0
$$
$$
\vdots
$$
$$
c_0\psi_0^{(m-1)}(t_0)+\dots+c_{m-1}\psi_{m-1}^{(m-1)}(t_0)=0
$$
 ma da [[ODE lineare]] sappiamo che esiste una soluzione diversa da $0$ per ogni $t$, quindi le equazioni sono nulle se e solo se $c_0=\dots=c_{m-1}=0\quad\square$