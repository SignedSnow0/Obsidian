---
subject: reti logiche
type: definizione
---
Una tabella della verità è una tabella usata per descrivere il comportamento di una [[Espressione booleana]].
Una tabella della verità ha $n+1$ colonne: $n$ per i bit di input e 1 per il bit in uscita, e ha $2^n$ righe per ogni possibile configurazione in ingresso (se [[Funzione completa]]) oppure di meno se [[Funzione incompleta]].

Una tabella della verità può descrivere correttamente una [[Rete Logica#Rete combinatoria]]
perchè il comportamento di una [[Rete Logica#Rete sequenziale]] dipende dai bit di stato e quindi non si può descrivere l'uscita in una sola colonna.

|$x_0$   |$\dots$ |$x_{n-1}$|$F(x_0,\dots,x_{n-1})$|
|:------:|:------:|:-------:|:--------------------:|
|$0$     |$\dots$ |$0$      |$F(0,\dots,0)$        |
|$\vdots$|$\ddots$|$\vdots$ |$\vdots$              |
|$1$     |$\dots$ |$1$      |$F(1,\dots,1)$        |