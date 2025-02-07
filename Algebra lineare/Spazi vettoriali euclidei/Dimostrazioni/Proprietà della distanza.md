---
subject: algebra lineare
type: dimostrazione
---
Sia $(V,\cdot)$ uno [[Spazio vettoriale euclideo|spazio vettoriale euclideo]], $x,y,z\in V$, allora
1. $d(x,y)\ge0$
2. $d(y,x)=d(x,y)$
3. $d(x,z)\le d(x,y)+d(y,z)$ ^a5b023
### Note
Il punto [[#^a5b023|3]] rappresenta una generalizzazione della [[Disuguaglianza triangolare|disuguaglianza triangolare]] in $\mathbb{R}^n$
# Dimostrazione
1. Deriva dalla definizione di [[Distanza|distanza]]
2. 
$$
d(y,x)=||y-x||=||-(x-y)||=||x-y||=d(x,y)
$$
3. 
$$
d(x,z)=||x-z||=||x-y+y-z||\le||x-y||+||y-z||=d(x,y)+d(y,z)\quad\square
$$