In Java vengono implementate istanze di [[Processi|threads]] grazie all'ereditarietà:
* Una classe può ereditare da *Thread*, allora avrà disponibile un metodo virtuale *run* dove verrà scritto il codice eseguito da un thread separato
* Se invece la classe implementa *Runnable* implementerà lo stesso metodo *run*, ma l'istanza dovrà essere incapsulata in un oggetto *Thread* per l'esecuzione

Come in [[Processi - Linux|c]] per aspettare la fine di un thread figlio si può chiamare *join* sull'oggetto.
![[Thread.png]]

Inoltre per garantire la [[Modello a memoria comune|mutua esclusione]] di sezioni critiche esiste la keyword *synchronized* che effettivamente implementa un [[Modello a memoria comune|mutex]] sulla risorsa.
![[Synchronized.png]]