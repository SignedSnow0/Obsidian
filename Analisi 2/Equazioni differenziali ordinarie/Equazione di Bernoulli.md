---
subject: analisi 2
type: procedimento
---
É un'[[Equazione differenziale|equazione differenziale]] del tipo
$$
x'(t)=a(t)x(t)+b(t)x^\alpha(t)
$$
con $\alpha\in\mathbb{R}\setminus\{0,1\}$ (dove $0,1$ sono riconducibile a un [[ODE lineare|equazione lineare]]).
## Metodo risolutivo
Se $x(t_0)\ne0$ poniamo
$$
x(t)^{-\alpha}x'(t)=a(t)x(t)^{1-\alpha}+b(t)
$$
ponendo $y(t)=x(t)^{1-\alpha}$ otteniamo il seguente [[Problema di Cauchy|problema di Cauchy]]
$$
\begin{cases}\frac{y'(t)}{1-\alpha}=a(t)y(t)+b(t)\\ y(t_0)=x_0^{1-\alpha}\end{cases}
$$
risolvendo $y(t)$ come un [[ODE lineare|equazione lineare]] troviamo poi $x(t)$ come
$$
x(t)=\begin{cases}y(t)^{\frac{1}{1-\alpha}}\quad x_0>0\\ -y(t)^{\frac{1}{1-\alpha}}\quad x_0<0\end{cases}
$$