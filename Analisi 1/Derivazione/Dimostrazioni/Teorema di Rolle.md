---
subject: analisi 1
type: dimostrazione
---
Sia $f\in\mathcal{C}([a,b])$, derivabile in $(a,b)$, se $f(a)=f(b)$, allora esiste $x_0\in(a,b):f'(x_0)=0$
# Dimostrazione
Per il teorema di Weierstrass esistono
$$
x_m\in[a,b]:f(x_m)=\min_{x\in[a,b]} f(x)=m,\quad x_M\in[a,b]:f(x_M)=\max_{x\in[a,b]} f(x)=M
$$
Allora $m\le f(a)=f(b)\le M$, quindi se $f(a)=f(b)<M$, allora $x_M$ è punto critico e per il [[Teorema di Fermat]] $f'(x_M)=0\quad\square$