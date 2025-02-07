---
subject: reti logiche
type: definizione
---
In una rete sequenziale asincrona lo stato futuro sovrascrive lo stato presente non appena è stato calcolato.
Il ciclo di esecuzione di una RSA è 
1. Partendo da uno stato stabile presente la rete cambia il valore di ingresso.
2. La rete calcola un nuovo stato futuro e dopo un ritardo di propagazione diventa il nuovo stato presente.
3. La rete calcola un nuovo valore di uscita in base all'ingresso e il nuovo stato.
4. Per rimanere stabile lo stato calcolato rimane sempre quello presente fino a un cambio di ingressi.

