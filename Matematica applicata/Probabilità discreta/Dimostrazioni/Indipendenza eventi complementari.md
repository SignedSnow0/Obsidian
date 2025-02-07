---
subject: matematica applicata
type: dimostrazione
---
Sia $S$ uno [[Spazio campione|spazio campione]], $E,F\subseteq S$ due [[Eventi indipendenti|eventi indipendenti]], allora anche $E^c,F^c$ sono [[Eventi indipendenti|indipendenti]].
# Dimostrazione
Dalla teoria degli insiemi abbiamo che $E^c\cap F^c=(E\cup F)^c$, allora
$$
P(E^c\cap F^c)=P((E\cup F)^c)=1-P(E\cup F)=1-[P(E)+P(F)-P(E\cap F)]
$$
dato che $E,F$ sono [[Eventi indipendenti|indipendenti]] si ha
$$
=1-P(E)-P(F)+P(E)P(F)=P(E^c)-P(F)(1-P(E))=P(E^c)-P(F)P(E^c)=
$$
$$
P(E^c)(1-P(F))=P(E^c)P(F^c)\quad\square
$$
