---
subject: analisi 1
type: dimostrazione
---
Sia $f,g\in\mathcal{C}([a,b])$, se $f(a)<g(a),\quad f(b)>g(b)$ allora esiste $x_0\in[a,b]:f(c)=g(c)$
# Dimostrazione
Sia $h(x)=f(x)-g(x)$, allora 
$$
h(x)\in\mathcal{C}([a,b]),\quad h(a)<0,\quad h(b)>0
$$ 
allora $h(x)$ soddisfa il [[Analisi 1/Continuità/Dimostrazioni/Teorema di Bolzano]], perciò
$$
\exists c\in[a,b]:h(x)=0=f(c)-g(c)\quad\square
$$
