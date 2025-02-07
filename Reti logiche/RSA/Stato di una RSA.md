---
subject: reti logiche
type: definizione
---
In una rete sequenziale asincrona non esistono componenti che "ricordano" lo stato della macchina in un preciso momento, ma lo stato è memorizzato grazie al ritardo di propagazione negli anelli in [[Retroazione]] di una RSA.

In poche parole una RSA è formate da una rete combinatoria che calcola costantemente i bit di [[Stato presente e futuro]] in base ai bit di stato e di ingresso e un altra rete combinatoria che calcola i bit di uscita in base ai soli bit di stato se nel modello di *Moore* o in base ai bit di stato e ingresso se nel modello di *Mealy*.