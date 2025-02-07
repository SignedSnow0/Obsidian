---
subject: analisi 2
type: dimostrazione
---
Sia un [[ODE lineare|equazione lineare]] omogenea, allora l'[[Integrale generale|integrale generale]] è un [[Sottospazio vettoriale|sottospazio vettoriale]] di $\mathcal{C}^{(m)}(I)$ di dimensione $m$.
# Dimostrazione
Iniziamo osservando che nel caso omogeneo l'integrale generale coincide con il [[Kernel|kernel]] della trasformazione lineare $T$ definito in [[Linearità delle ODE lineari]], già sappiamo che il [[Kernel|kernel]] è un [[Sottospazio vettoriale|sottospazio vettoriale]], bisogna trovarne la dimensione.
Consideriamo i seguenti problemi di Cauchy
$$
\begin{cases}Tx=0\\x(t_0)=1\\\vdots\\x^{(m-1)}(t_0)=0\end{cases}\quad\dots\quad\begin{cases}Tx=0\\x(t_0)=0\\\vdots\\x^{(m-1)}(t_0)=1\end{cases}
$$
in modo da assomigliare una [[Base canonica]], chiamiamo $\phi_0\dots,\phi_{m-1}$ le [[Soluzione massimale]] di questi problemi e dimostriamo che sono una [[Base]] per $T$.
Sia $x\in\mathcal{C}^m(I):Tx=0$, sia
$$
y=x(t_0)\phi_0+\dots+x^{(m-1)}(t_0)\phi_{m-1}
$$
consideriamo il problema
$$
\begin{cases}Tz=0\\z(t_0)=x(t_0)\\\vdots\\ z^{(m-1)}(t_0)=x^{(m-1)}(t_0)\end{cases}
$$
allora sia $x$ che $y$ sono [[Soluzione massimale]] e quindi $x=y$, ma $y$ è [[Combinazione lineare]] di $\phi_0,\dots,\phi_{m-1}$ e quindi lo è anche $x$.
Sia ora $c_0,\dots,c_{m-1}\in\mathbb{R}:$
$$
c_0\phi_0(t)+\dots+c_{m-1}\phi_{m-1}(t)=0\quad\forall t\in I
$$
allora
$$
c_0\phi_0'(t)+\dots+c_{m-1}\phi_{m-1}'(t)=0\quad\forall t\in I
$$
$$
\vdots
$$
$$
c_0\phi_0^{(m-1)}(t)+\dots+c_{m-1}\phi_{m-1}^{(m-1)}(t)=0\quad\forall t\in I
$$
Prendendo $t=t_0$ si ottiene
$$
c_0=\dots=c_{m-1}=0
$$
e quindi $\phi_0,\dots,\phi_{m-1}$ sono una base di dimensione $m$ per $T\quad\square$