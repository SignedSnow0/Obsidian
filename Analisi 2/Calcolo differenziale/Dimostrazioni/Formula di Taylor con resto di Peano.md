---
subject: analisi 2
type: dimostrazione
---
Sia $A\subseteq\mathbb{R}^n$ aperto, $f\in\mathcal{C}^k(A),x^0\in A$, introduciamo il seguente polinomio
$$
P(x_1,\dots,x_n)=f(x_0)+\sum_{j=1}^{n}\frac{\partial f}{\partial x_j}(x^0)(x_j-x_j^0)+\dots
$$
$$
+\frac{1}{k!}\sum_{j_1=1}^{n}\dots\sum_{j_k=1}^{n}\frac{\partial^k f}{\partial x_{j_1}\dots\partial x_{j_k}}(x^0)(x_{j_1}-x_{j_1}^0)\dots(x_{j_k}-x_{j_k}^0)
$$
Chiamiamo $P$ il polinomio di Taylor di grado non superiore a $k$ centrato in $x^0$ per $f$, e vale
$$
f=P+o(||x-x^0||^k)
$$
# Dimostrazione
Sia $k=2, r\in\mathbb{R}^+:B(x^0,r)\subseteq A$, per $x\in B(x^0,r)$ poniamo
$$
F:[0,1]\to\mathbb{R},F(t)=f(x^0,t(x-x^0))
$$
ricordando [[Teorema del valor medio|Teorema del valor medio]] si ha 
$$
F'(t)=\sum_{j=1}^{n}\frac{\partial f}{\partial x_j}(x^0+t(x-x^0))(x_j-x^0_j)
$$
e continuando 
$$
F''(t)=\sum_{j_1=1}^{n}\sum_{j_2=1}^{n}\frac{\partial^2 f}{\partial x_{j_1}\partial x_{j_2}}(x^0+t(x-x^0))(x_{j_1}-x_{j_1}^0)(x_{j_2}-x_{j_2}^0))
$$
infine applicando il [[Formula di Taylor con resto di Peano#Lemma]] si ha per un certo $c\in(0,1)$
$$
f(x)=F(1)=F(0)+F'(0)+\frac{F''(c(x))}{2}=
$$
$$
f(x^0)+\sum_{j=1}^{n}\frac{\partial f}{\partial x_j}(x^0)(x_j-x_j^0)+\frac{1}{2}\sum_{j_1=1}^{n}\sum_{j_2=1}^{n}\frac{\partial^2 f}{\partial x_{j_1}\partial x_{j_2}}(x^0+c(x)(x-x^0))(x_{j_1}-x_{j_1}^0)(x_{j_2}-x_{j_2}^0)=
$$
$$
P(x)+\frac{1}{2}\sum_{j_1=1}^{n}\sum_{j_2=1}^{n}\left[\frac{\partial^2 f}{\partial x_{j_1}\partial x_{j_2}}(x^0+c(x)(x-x^0))-\frac{\partial^2 f}{\partial x_{j_1}\partial x_{j_2}}(x^0)\right](x_{j_1}-x_{j_1}^0)(x_{j_2}-x_{j_2}^0)
$$
dove
$$
P(x)=f(x^0)+\sum_{j=1}^{n}\frac{\partial f}{\partial x_j}(x^0)(x_j-x_j^0)+\frac{1}{2}\sum_{j_1=1}^{n}\sum_{j_2=1}^{n}\frac{\partial^2 f}{\partial x_{j_1}\partial x_{j_2}}(x^0)(x_{j_1}-x_{j_1}^0)(x_{j_2}-x_{j_2}^0)
$$
proviamo ora che $f(x)-P(x)=o(||x-x^0||^2)$
Sia $\epsilon,\eta\in\mathbb{R}^+$, poichè $f\in\mathcal{C}^2$
$$
\exists\delta(\eta)>0:y\in B(x^0,\delta(\eta))\implies\left|\frac{\partial^2 f}{\partial x_{j_1}\partial x_{j_2}}(y)-\frac{\partial^2 f}{\partial x_{j_1}\partial x_{j_2}}(x^0)\right|<\eta
$$
inoltre se $x\in B(x^0,\delta(\eta))\implies ||x-x^0||<\delta(\eta)$
dalle precedenti implicazioni segue che 
$$
|f(x)-P(x)|\le\frac{1}{2}\eta\sum_{j_1=1}^{n}\sum_{j_2=1}^{n}|x_{j_1}-x_{j_1}^0||x_{j_2}-x_{j_2}^0|\le \frac{n^2}{2}\eta||x-x^0||^2
$$
allora segue che se $x\in B(x^0,\delta(\eta))\setminus\{x^0\}$
$$
\frac{|f(x)-P(x)|}{||x-x^0||^2}\le \frac{n^2}{2}\eta
$$
perciò per $\frac{n^2}{2}\eta<\epsilon$
$$
\frac{|f(x)-P(x)|}{||x-x^0||^2}\le\epsilon\quad\square
$$

## Lemma
Sia $F\in\mathcal{C}^2([0,1])$, allora esiste $c\in[0,1]:$
$$
F(1)=F(0)+F'(0)+\frac{F''(c)}{2}
$$
## Dimostrazione
Sia $r:[0,1]\to\mathbb{R},r(x)=F(x)-F(0)-F'(0)x$, allora $r\in\mathcal{C}^2([0,1])$, allora applicando [[Teorema di Cauchy]] a $r,g(x)=x^2$ abbiamo 
$$
\exists c_1\in(0,1):g'(c_1)[r(1)-r(0)]=r'(c_1)[g(1)-g(0)]
$$
da cui 
$$
F(1)-F(0)-F'(0)=r(1)=\frac{r'(c_1)}{2c_1}
$$
applicando di nuovo lo stesso teorema a $r',g'$ abbiamo che
$$
F(1)-F(0)-F'(0)=\frac{r''(c)}{2}=\frac{F''(c)}{2}\quad\square
$$