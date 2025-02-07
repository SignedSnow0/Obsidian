---
subject: reti logiche
type: definizione
---
### Alea dinamica
In una RSA un'alea dinamica è il momento in cui l'uscita prima di assestarsi sul nuovo valore stabile varia più volte.
Di solito la causa di un alea dinamica è il diverso tempo di calcolo per i bit dell'uscita, fortunatamente però sintesi in [[Espressione canonica]] non presentano mai alee dinamiche.
### Alea statica
In una RSA un'alea statica è il momento in cui l'uscita cambia temporaneamente di valore quando invece non dovrebbe.
Per evitare alee statiche bisogna fare coperture ridondanti di [[Mappa di Karnaugh]] cioè bisogna creare [[Raggruppamento rettangolare]] a cavallo di due raggruppamenti adiacenti che non si intersecano cioè la sintesi in [[Espressione canonica]] avrà tutti i [[Implicato primo]] o [[Implicante primo]].