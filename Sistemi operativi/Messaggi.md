I processi nei sistemi operativi moderni non hanno memoria in comune, perciò per interagire fra di loro hanno bisogno di un meccanismo indipendente da variabili di stato.
Allora sono necessarie operazioni fornite dal sistema operativo per mandare/ricevere informazioni fra processi concorrenti.
Questa comunicazione è divisa in due tipologie:
* Diretta: il messaggio viene mandato direttamente ad un unico destinatario.
* Indiretta: il messaggio viene mandato ad un intermediario dal quale poi verrà letto da ogni processo iscritto ad esso.

![[Messaggi.excalidraw]]

Inoltre la comunicazione è caratterizzata dalla capacità del canale di comunicazione:
* Se il canale non ha capacità di buffering ogni invio/ricezione del messaggio sospende i processi finchè non sono entrambi pronti allo scambio.
* Se invece il canale ha capacità di buffering le chiamate non sono sospensive, a meno che il canale non sia pieno/vuoto.

> [!definition] Pipe
> Il pipe è un canale di comunicazione indiretto, che permette quindi comunicazione molti a molti e con capacità di buffering.