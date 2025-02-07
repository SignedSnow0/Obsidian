---
subject: analisi 2
type: dimostrazione
---
Data [[ODE lineare|equazione lineare]] a coefficienti costanti di secondo ordine
$$
x''(t)=a_0x(t)+a_1x'(t)
$$
sia $P(\lambda)=\lambda^2-a_1\lambda-a_0$ il suo [[Polinomio caratteristico di un ODE lineare a coefficienti costanti|polinomio caratteristico]], allora:
1. Se $P$ ha due zeri reali e distinti $\lambda_0,\lambda_1$, allora $\psi_0(t)=e^{\lambda_0t},\psi_1(t)=e^{\lambda_1t}$ costituiscono un [[Sistema fondamentale di soluzioni|sistema fondamentale di soluzioni]]
2. Se $P$ ha un unico zero reale $\lambda_0$ di [[Molteplicità algebrica|molteplicità algebrica]] 2 le funzioni $\psi_0(t)=e^{\lambda_0t},\psi_1(t)=te^{\lambda_0 t}$ costituiscono un [[Sistema fondamentale di soluzioni|sistema fondamentale di soluzioni]]
3. Se $P$ ha degli zeri complessi coniugati $\alpha\pm i\beta$, le funzioni $\psi_0(t)=e^{\alpha t}\cos(\beta t),\psi_1(t)=e^{\alpha t}\sin(\beta t)$ costituiscono un [[Sistema fondamentale di soluzioni|sistema fondamentale di soluzioni]]
# Dimostrazione
Sia 1 verificato, allora [[Soluzione di ODE a coefficienti costanti|sappiamo che]] $\psi_0,\psi_1$ sono soluzioni.
Allora $\forall t\in I$
$$
w(\psi_0,\psi_1)(t)=\det\begin{pmatrix}e^{\lambda_0t}&e^{\lambda_1t}\\\lambda_0e^{\lambda_0t}&\lambda_1e^{\lambda_1t}\end{pmatrix}=(\lambda_1-\lambda_0)e^{(\lambda_0+\lambda_1)t}\ne0
$$
perchè $\lambda_0\ne\lambda_1$
Sia 2 verificato, $\psi_0$ è soluzione, dato che $\lambda_0$ è l'unico zero di d $P$ con molteplicità 2
$$
P(\lambda)=(\lambda-\lambda_0)^2=\lambda^2-2\lambda_0\lambda+\lambda_0^2
$$
dunque $\forall t\in I$
$$
\psi_1''(t)-a_1\psi_1'(t)-a_0\psi_1(t)=\lambda_0(2+\lambda_0t)e^{\lambda_0t}-2\lambda_0(1+t\lambda_0)e^{\lambda_0t}+\lambda_0^2te^{\lambda_0t}=0
$$
inoltre 
$$
w(\psi_0,\psi_1)(t)=\det\begin{pmatrix}e^{\lambda_0t}&te^{\lambda_0t}\\\lambda_0e^{\lambda_0t}&(1+t\lambda_0)e^{\lambda_0t}\end{pmatrix}=e^{2\lambda_0t}\ne0
$$
Sia 3 verificato, visto che $\alpha\pm i\beta$ sono gli zeri si ha $\forall\lambda\in\ C$
$$
P(\lambda)=(\lambda-\alpha-i\beta)(\lambda-\alpha+i\beta)=\lambda^2-2\alpha\lambda+\alpha^2+\beta^2
$$
allora $\forall t\in I$
$$
\psi_0''(t)-a_1\psi_0'(t)-a_0\psi_0(t)=\psi_0''(t)-2\alpha\psi_0'(t)+(\alpha^2+\beta^2)\psi_0(t)=
$$
$$
(\alpha^2-\beta^2)e^{\alpha t}\cos(\beta t)-2\alpha\beta e^{\alpha t}\sin(\beta t)-2\alpha[\alpha e^{\alpha t}\cos(\beta t)-\beta e^{\alpha t}\sin(\beta t)]+(\alpha^2+\beta^2)e^{\alpha t}\cos(\beta t)=0
$$
$\psi_1$ si verifica in modo analogo, infine abbiamo che
$$
w(\psi_0,\psi_1)(t)=\det\begin{pmatrix}e^{\alpha t}\cos(\beta t)&e^{\alpha t}\sin(\beta t)\\\alpha e^{\alpha t}\cos(\beta t)-\beta e^{\alpha t}\sin(\beta t)&\alpha e^{\alpha t}\sin(\beta t)+\beta e^{\alpha t}\cos(\beta t)\end{pmatrix}=\beta e^{2\alpha t}\ne 0\quad\square
$$