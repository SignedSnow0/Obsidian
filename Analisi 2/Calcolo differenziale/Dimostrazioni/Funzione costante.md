---
subject: analisi 2
type: dimostrazione
---
Sia $A\subseteq{R}^n$ [[Insieme connesso per archi|connesso per archi]], $f\in\mathcal{C}^1(A):\nabla f(x)=O\quad\forall x\in A$, allora $f$ è costante in $A$
# Dimostrazione
Sia $x,y\in A$, per il [[Funzione costante#Lemma]] esiste
$$
a,b\in\mathbb{R},a<b:\alpha([a,b])\subseteq A,\alpha(a)=x,\alpha(b)=y
$$
sia
$$
g:[a,b]\to\mathbb{R},\quad g(t)=f(\alpha(t))
$$
allora $g\in\mathcal{C}^1$ e 
$$
g'(t)=\nabla f(\alpha(t))\cdot\alpha'(t)=0\quad\forall t\in[a,b]
$$
segue allora che $g$ è costante, perciò
$$
f(x)=f(\alpha(a))=g(a)=g(b)=f(\alpha(b))=f(y)\quad\square
$$

# Lemma
Sia $A\subseteq\mathbb{R}^n$ [[Insieme connesso per archi]], allora comunque si prendano $x,y\in A$ esiste un cammino continuo con sostegno in $A$ che ha $x$ come primo estremo e $y$ come secondo.