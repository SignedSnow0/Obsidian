---
subject: matematica applicata
type: dimostrazione
---
Dato uno [[Spazio campione|spazio campione]] $S$, una [[Partizione|partizione]] di $S$ e un [[Evento|evento]] $E$ tale che $P(E)\ne0$, si ha
$$
P(H_j|E)=\frac{P(E|H_j)P(H_j)}{\displaystyle\sum_{j=1}^nP(E|H_j)P(H_j)}
$$
# Dimostrazione
Usando la definizione di [[Probabilità condizionata|probabilità condizionata]] si ha che 
$$
P(H_j|E)P(E)=P(E\cap H_j)=P(E|H_j)P(H_j)
$$
quindi
$$
P(H_j|E)P(E)=P(E|H_j)P(H_j)
$$
riordinando i termini
$$
P(H_j|E)=\frac{P(E|H_j)P(H_j)}{P(E)}
$$
infine utilizzando il [[Teorema delle probabilità totali|teorema dell probabilità totali]]
$$
P(H_j|E)=\frac{P(E|H_j)P(H_j)}{\displaystyle\sum_{j=1}^nP(E|H_j)P(H_j)}\quad\square
$$