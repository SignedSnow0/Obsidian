---
subject: analisi 2
type: procedimento
---
Consideriamo l'[[ODE lineare|equazione lineare]]
$$
x''(t)=a_0(t)x(t)+a_1(t)x'(t)+b(t)
$$
supponiamo di conoscere un [[Sistema fondamentale di soluzioni|sistema fondamentale di soluzioni]] $\{\psi_0,\psi_1\}$ dell'[[ODE lineare omogenea associata|equazione omogenea associata]], cerchiamo allora una soluzione $\phi$ della forma
$$
\phi(t)=c_0(t)\psi(t)+c_1(t)\psi_1(t)
$$
con  $c_0,c_1\in\mathcal{C}^1(I)$, si ha allora 
$$
\phi'(t)=c'_0(t)\psi_0(t)+c_1'(t)\psi_1(t)+c_0(t)\psi_0'(t)+c_1(t)\psi_1'(t)
$$
Imponiamo ora la prima condizione
$$
c'_0(t)\psi_0(t)+c'_1(t)\psi_1(t)=0
$$
allora segue che
$$
\phi''-a_1\phi'-a_0\phi=c'_0\psi'_0+c'_1\psi'_1
$$
riconducendoci quindi al sistema di incognite $c_0'(t),c_1'(t)$
$$
\begin{cases}c'_0(t)\psi_0(t)+c'_1(t)\psi_1(t)=0\\c'_0(t)\psi'_0(t)+c'_1(t)\psi'_1(t)=b(t)\end{cases}
$$
per il [[Teorema del Wronskiano|teorema del wronskiano]] il sistema è univocamente risolubile per ogni $t\in I$ e
$$
c'_0(t)=-\frac{b(t)\psi_1(t)}{w(\psi_0,\psi_1)(t)},\quad c'_1(t)=\frac{b(t)\psi_0(t)}{w(\psi_0,\psi_1)(t)}
$$
allora con  $c_0,c_1$ primitive di $c_0',c_1',\quad\phi$ è soluzione.