---
subject: reti logiche
type: definizione
---
Un latch SR è una RSA che permette di ricordare lo stato di un bit per un tempo indefinito.
* L'ingresso S imposta l'uscita Q a 1 se attivato.
* L'ingresso R imposta l'uscita Q a 0 se attivato.

Per il corretto comportamento di un SR latch gli ingressi S e R non possono mai essere attivi contemporaneamente.

Esistono due [[Ingresso asincrono]] che agiscono sul valore di Q
* $\overline{\text{PRE}}$ che imposta Q a 1.
* $\overline{\text{CLR}}$ che imposta Q a 0.