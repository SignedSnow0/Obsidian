---
subject: matematica applicata
type: dimostrazione
---
Sia $S$ uno [[Spazio campione|spazio campione]] e $E,F\subseteq S$ due suoi [[Evento|eventi]], allora
1. $P(E^c)=1-P(E)$
2. $P(\emptyset)=0$
3. Se $E\subseteq F$,allora $P(E)\le P(F)$
4. $P(E\cup F)=P(E)+P(F)-P(E\cap F)$

# Dimostrazione
1. Per  l'[[Probabilità di Kolmogorov|assioma 1]] sappiamo che $P(E^c\cup E)=P(S)=1$, e per l'[[Probabilità di Kolmogorov|assioma 3]] sappiamo che $P(E^c\cup E)=P(E^c)+P(E)$, allora 
$$
1=P(E^c)+P(E)\implies P(E^c)=1-P(E)
$$
2. Sappiamo che $\emptyset^c=S$, quindi per proprietà 1
$$
P(\emptyset)=P(S^c)=1-1=0
$$
3. Notiamo che $F=E\cup(E^c\cap F)$, allora
$$
P(F)=P(E)+P(E^c\cap F)\ge P(E)
$$
4. Sia $A_1=E\cap F^c,A_2=E\cap F,A_3=F\cap E^c$, allora $E=A_1\cup A_2,F=A_2\cup A_3$, perciò
$$
P(E)=P(A_1)+P(A_2),\quad P(F)=P(A_2)+P(A_3),\quad P(E\cup F)=P(A_1)+P(A_2)+P(A_3)
$$
allora
$$
P(E)+P(F)-P(E\cap F)=P(A_1)+P(A_2)+P(A_2)+
$$
$$
P(A_3)-P(A_2)=P(A_1)+P(A_2)+P(A_3)=P(E\cup F)\quad\square
$$