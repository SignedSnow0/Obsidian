Iniziamo ricordando l'equazione di Dirac per una particella nel vuoto
> [!definition] Equazione di Dirac
> $$
> i\hbar\gamma^\mu\partial_\mu\psi-mc\psi=0
> $$

dove $\psi$ è un bispinore
$$
\psi=\begin{pmatrix}\psi_1\\\psi_2\\\psi_3\\\psi_4\end{pmatrix}\in\mathbb{C}^4
$$
e $\gamma^\mu$ sono le matrici gamma in forma controvariante.

---
Iniziamo ora risolvendo l'equazione di Dirac per una particella che non ha momento.
Allora espandendo l'equazione si ha
$$
\frac{1}{c}\gamma^0\frac{\partial\psi}{\partial t}+\gamma^1\frac{\partial\psi}{\partial x}+\gamma^2\frac{\partial\psi}{\partial y}+\gamma^3\frac{\partial\psi}{\partial z}=-\frac{imc}{\hbar}\psi
$$
dato che sappiamo che il momento è esattamente $\vec{0}$ allora per il principio di incertezza possiamo aspettarci di non sapere niente sulla posizione, quindi
$$
\frac{\partial\psi}{\partial x}=\frac{\partial\psi}{\partial y}=\frac{\partial\psi}{\partial z}=0
$$
abbiamo quindi
$$
\frac{1}{c}\gamma^0\frac{\partial\psi}{\partial t}=-\frac{imc}{\hbar}\psi
$$
che in forma estesa è
$$
\begin{bmatrix}1&0&0&0\\0&1&0&0\\0&0&-1&0\\0&0&0&-1\end{bmatrix}\frac{\partial}{\partial t}\begin{bmatrix}\psi_1\\\psi_2\\\psi_3\\\psi_4\end{bmatrix}=-\frac{imc^2}{\hbar}\begin{bmatrix}\psi_1\\\psi_2\\\psi_3\\\psi_4\end{bmatrix}
$$
espandendo i calcoli arriviamo a due equazioni correlate
$$
\frac{\partial}{\partial t}\begin{bmatrix}\psi_1\\\psi_2\end{bmatrix}=-\frac{imc^2}{\hbar}\begin{bmatrix}\psi_1\\\psi_2\end{bmatrix}\quad\psi_3=\psi_4=0
$$
$$
\frac{\partial}{\partial t}\begin{bmatrix}\psi_3\\\psi_4\end{bmatrix}=\frac{imc^2}{\hbar}\begin{bmatrix}\psi_3\\\psi_4\end{bmatrix}\quad\psi_1=\psi_2=0
$$
risolvendo per $\psi$ si ha
$$
\psi=\begin{bmatrix}a\\b\\0\\0\end{bmatrix}\exp\left(-\frac{imc^2}{\hbar}t\right)\quad|a|^2+|b|^2=1
$$
$$
\psi=\begin{bmatrix}0\\0\\c\\d\end{bmatrix}\exp\left(\frac{imc^2}{\hbar}t\right)\quad|c|^2+|d|^2=1
$$
che sono le equazioni  dell'elettrone e positrone.
Continuiamo ora considerando solo l'elettrone
$$
\psi=\begin{bmatrix}a\\b\end{bmatrix}\exp\left(-\frac{imc^2}{\hbar}t\right)
$$
pensando $a$ e $b$ come combinazione lineare degli spin possibili di un elettrone si ha
$$
a\begin{bmatrix}1\\0\end{bmatrix}+b\begin{bmatrix}0\\1\end{bmatrix}
$$
allora possiamo vedere che a e b sono le probabilità di trovare l'elettrone in spin up o down.

---
Dimostriamo ora che il campo di Dirac ha simmetria di fase locale, cioè se un'onda è trasformata nella fase ogni quantità osservabile di essa rimane invariata.
> [!definition] Trasformazione di fase
> Data un equazione d'onda $\psi$ si ha che $\psi'$ è una trasformazione di fase se
> $$
> \psi'=\e^{i\theta}\psi
> $$