---
subject: matematica applicata
type: definizione
---
Dato uno [[Spazio campione|spazio campione]] $S$ e un [[Evento|evento]] $E\subseteq S$, si associa ad $E$ il numero razionale detto probabilità
$$
P(E)=\frac{\text{numero di esiti in } E}{\text{numero di esiti in } S}
$$
la definizione è valida però solo se il numero di [[Esito di un esperimento|esiti]] in $
S$ è finiti e se sono tutti equiprobabili.


### Derivazione
Sia $S$ uno [[Spazio campione|spazio campione]] con $n$ [[Esito di un esperimento|esiti]] equiprobabili, allora per il [[Probabilità di Kolmogorov|terzo assioma]] della [[Probabilità di Kolmogorov|probabilità di Kolmogorov]] abbiamo che 
$$
1=P(S)=P\left(\bigcup_{j=1}^ne_j\right)=\sum_{j=1}^nP(e_j)=nP(e_j)\implies P(e_j)=\frac{1}{n}
$$
Dato un [[Evento|evento]] $E\subseteq S,E=\{e_1,\dots,e_k\}$ abbiamo che
$$
P(E)=P\left(\bigcup_{j=1}^ke_j\right)=\sum_{j=1}^k\frac{1}{n}=\frac{k}{n}\quad\square
$$