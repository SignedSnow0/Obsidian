---
subject: reti logiche
type: definizione
---
In una [[Mappa di Karnaugh]] un raggruppamento rettangolare è un raggruppamento di celle adiacenti dello stesso valore.
Due celle sono adiacenti se condividono un lato (due celle in diagonale non sono adiacenti) anche tra due tabelle se la mappa e a 5 o 6 variabili.
Un raggruppamento rettangolare è valido se racchiude un numero di celle in potenze di 2, e in quel caso il [[Mintermine]] o [[Maxtermine]] avrà $n-m$ variabili, dove $n$ è il numero di bit in input e $m$ è l'esponente del raggruppamento rettangolare.
Perciò per avere una vera [[Espressione canonica]] è importante prendere solamente i raggruppamenti più grandi possibili per generare [[Implicato primo]] o [[Implicante primo]].
Infine per evitare [[Alea statica]] è utile avere coperture ridondanti a cavallo di due raggruppamenti adiacenti che non si intersecano.