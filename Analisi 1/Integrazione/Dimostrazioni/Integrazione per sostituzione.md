---
subject: analisi 1
type: dimostrazione
---
Sia $f(y)$ integrabile su $J$, $F(y)$ una sua primitiva, sia $\phi(x)$ derivabile su $I$ con immagine in $J$, allora $f(\phi(x))\phi'(x)$ è integrabile in $I$ e si ha
$$
\int f(\phi(x))\phi'(x)dx=F(\phi(x))+c
$$
# Dimostrazione
Ricordando la [[Analisi 1/Derivazione/Dimostrazioni/Chain rule]]
$$
\frac{d}{dx}F(\phi(x))=\frac{dF}{dy}(\phi(x))\frac{d\phi}{dx}(x)=f(\phi(x))\phi'(x)
$$
Perciò $F(\phi(x))$ è primitiva di $f(\phi(x))\phi'(x)\quad\square$