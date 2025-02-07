---
subject: analisi 1
type: dimostrazione
---
Sia $f\in\mathcal{C}([a,b])$, derivabile in $(a,b)$, allora esiste $x_0\in(a,b):\frac{f(b)-f(a)}{b-a}=f'(x_0)$
# Dimostrazione
Sia $h(x)=f(x)+\frac{f(b)-f(a)}{b-a}(x-a)$, allora $h(a)=f(a),h(b)=f(a)$, perciò per il [[Teorema di Rolle]] esiste $x_0\in(a,b)$ tale che
$$
h'(x_0)=f'(x_0)-\frac{f(b)-f(a)}{b-a}=0\quad\square
$$