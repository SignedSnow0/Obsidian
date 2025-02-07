---
subject: fondamenti di telecomunicazioni
---
La conversione di un segnale analogico a digitale è divisa in 3 parti fondamentali
* Campionamento $x\to x_n$
* Quantizzazione $x_n\to q_n$
* Codifica $q_n\to \left\{b_n^1,\dots,b_n^l\right\}$
---
### Campionamento
La fase di campionamento trasforma il segnale tempo continuo in un segnale tempo discreto: una rete [[Serie temporale|campionerà]] il segnale ad una frequenza costante $f_c$ ottenendo la [[Serie temporale|serie temporale]] $x_n$, inoltre per il [[Teorema di Shannon|teorema di Shannon]] se il segnale non supera la [[Teorema di espansione di Shannon|frequenza di Nyquist]] non si ha perdita di dati nel processo.

---
### Quantizzazione
La [[Serie temporale|serie temporale]] ottenuta dalla fase di campionamento deve essere espressa in quantità di risoluzione finita, perciò ogni termine $x_n$ viene correlato ad un valore $q_n$ all'interno dell'intervallo di dinamica $[-M,M]$, ogni quantizzatore ha differenze in numero di intervalli, distribuzione di essi e numero di bit usato per ognuno di essi.
L'operazione di quantizzazione non è reversibile e porta un errore medio pari alla differenza fra il valore iniziale e finale chiamato errore di quantizzazzione. 
$$
e_n=x_n-q_n
$$

---
### Codifica
Dalla fase di quantizzazione si ha come risultato una serie $q_n$ di valori discreti divisi in $L$ possibili intervalli, ognuno di questi valori verrà associato ad una parola di $l$ bit con 
$$
l\ge\log_2L
$$
esistono diversi tipi di codifica, alcuni permettono ridondanza contro errori di trasmissione, altri compressione dei dati con o senza perdita di informazione.