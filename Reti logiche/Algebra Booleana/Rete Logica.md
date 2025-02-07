---
subject: reti logiche
type: definizione
---
Una rete logica è un modello che permette di rappresentare elaborazioni di segnali attraverso gate per determinare
* Che struttura porta a un determinato comportamento (sintesi)
* Che comportamento ha una struttura (analisi)

### Rete combinatoria
Una rete combinatoria è un particolare tipo di rete logica che porta una particolare sequenza in ingresso a una particolare sequenza di uscite in maniera simile a una funzione matematica.

Il modello standard di una rete combinatoria è rappresentabile con un set di bit in ingresso e un set di bit di uscita che sono calcolati nella rete stessa.

### Rete sequenziale
Una rete sequenziale asincrona è un particolare tipo di rete che per produrre un uscita ha bisogno oltre che a un ingresso un ulteriore set di bit che indicano lo stato attuale in cui si trova.

Le reti sequenziali asincrone sono modellate con due reti combinatorie che calcolano i bit di uscita e i bit di stato disposti in retroazione, perciò gli input della rete sono i veri e propri bit di ingresso più i bit necessari per rappresentare lo stato attuale, mentre in uscita ci sono solo i bit di output.