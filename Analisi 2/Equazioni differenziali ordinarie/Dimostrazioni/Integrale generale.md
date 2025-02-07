---
subject: analisi 2
type: dimostrazione
---
Presa un [[ODE lineare|equazione lineare]], sia $\{\psi_0,\dots,\psi_{m-1}\}$ un [[Sistema fondamentale di soluzioni|sistema fondamentale di soluzioni]] per l'[[ODE lineare omogenea associata|omogenea associata]] e $\phi$ una [[Soluzione massimale|soluzione massimale]] per $x$, allora l'integrale generale coincide con
$$
\{c_0\psi_0+\dots+c_{m-1}\psi_{m-1}+\phi|c_0,\dots,c_{m-1}\in\mathbb{R}\}
$$
# Dimostrazione
Sia $x=c_0\psi_0+\dots+c_{m-1}\psi_{m-1}+\phi$ (combinazione lineare), allora visto che $T$ è lineare si ha
$$
Tx=c_0T\psi_0+\dots+c_{m-1}T\psi_{m-1}+T\phi=b
$$
Viceversa sia ora $x$ [[Soluzione massimale]], allora
$$
T(x-\phi)=b-b=0
$$
perciò $x-\phi$ è [[Soluzione massimale]] dell'[[ODE lineare omogenea associata]], quindi esistono $c_0,\dots,c_{m-1}\in\mathbb{R}:$
$$
x-\phi=c_0\psi_0+\dots+c_{m-1}\psi_{m-1}\quad\square
$$