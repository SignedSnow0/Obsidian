---
subject: matematica applicata
type: dimostrazione
---
Dato uno [[Spazio campione|spazio campione]] $S$, un [[Evento|evento]] $E\subseteq S$, una [[Partizione|partizione]] di $S$, allora
$$
P(E)=\sum_{k=1}^nP(E|H_k)P(H_k)
$$

# Dimostrazione
Notiamo che
$$
E=(E\cap H_1)\cup\dots\cup(E\cap H_n)
$$
inoltre dato che $H_i\cap H_j=\emptyset$ per [[Partizione|definizione]], si ha che
$$
(E\cap H_i)\cap(E\cap H_j)=\emptyset\quad i\ne j
$$
quindi $E\cap H_i,\space E\cap H_j$ sono disgiunti, allora per l'[[Probabilità di Kolmogorov|assioma 3]]
$$
P(E)=P((E\cap H_i)\cup\dots\cup(E\cap H_n))=P(E\cap H_1)+\dots+P(E\cap H_n)
$$
infine per definizione di [[Probabilità condizionata]] si ha che $P(E\cap H_i)=P(E|H_i)P(H_i)$, quindi 
$$
P(E)=\sum_{j=1}^nP(E|H_j)P(H_j)\quad\square
$$