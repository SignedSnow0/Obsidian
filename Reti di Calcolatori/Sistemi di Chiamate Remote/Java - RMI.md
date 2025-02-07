## Java: Oggetti, Classi e Interfacce
In java, a runtime, oltre agli oggetti vengono istanziate anche classi ed interfacce:
* Un **oggetto** è creato da una sola classe che ne definisce il tipo, all'interno dell'oggetto sono memorizzate tutte le variabili (non statiche).
* Una **classe** invece viene memorizzata se almeno un oggetto di quel tipo è utilizzato, la classe contiene tutte le implementazioni dei metodi, dati statici e riferimenti alle interfacce che implementa.
* Le **interfacce** invece sono tipi di metalivello che contengono riferimenti a tutti gli oggetti che la implementano.
## Java RPC: RMI
In java il meccanismo di **Remote Method Invocation** permette di chiamare metodi di oggetti presenti su un altra macchina attraverso un riferimento remoto ad esso.
* Il meccanismo di invocazione è del tutto trasparente attraverso l'utilizzo di [[Generalitá#RPC - Stub|stub e skeleton]] dalla parte di client e server rispettivamente.
* È aggiunto un livello subito sopra al trasporto chiamato **Remote Reference Layer** che si occupa della gestione dei **riferimenti remoti** e parametri.
*  È presente un sistema di nomi per il binding dinamico dei servizi chiamato **RMIRegistry**
## Chiamate remote
In RMI la chiamata ad un oggetto remoto è effettuata in maniera trasparente:
* Attraverso l'**RMIRegistry** il client ottiene lo stub, un riferimento remoto al servizio ricercato.
* Il cliente effettua la chiamata sullo **stub** in maniera **sincrona** e **bloccante**, con semantica **at most once** grazie al trasporto TCP.
* Il **RRL** si occupa del marshalling di parametri e unmarshalling dal lato del server.
* Attraverso lo **skeleton** il server riceve la chiamata in maniera trasparente, come se fosse dalla stessa macchina.
* La risposta è passata al cliente in maniera trasparente.

Nonostante l'alto livello di astrazione ci sono alcune differenze rispetto alla programmazione "normale":
* Le interfacce dei servizi devono estendere *java.rmi.Remote*.
* Ogni metodo del servizio deve poter lanciare *java.rmi.RemoteException*.
* La classe implementativa del server deve estendere *java.rmi.UnicastRemoteObject*.
* I parametri di ingresso/uscita devono implementare *java.io.Serializable* se passati per valore o *java.rmi.Remote* se passati per riferimento remoto.
* Stub e skeleton devono essere disponibili a runtime dal server per la distribuzione verso il client.
## RMIRegistry
Il RMIRegistry è il servizio di nomi implementato per i servizi RMI, alla base è una tabella di coppie **nome, riferimento** dove il nome consiste in una striga arbitraria, mentre il riferimento è un riferimento (anche remoto) all'oggetto che implementa il servizio. Di default il registro ascolta sulla porta 1099, e fornisce i seguenti servizi:
* *bind/rebind* di servizi su un nome.
* *unbind* di un servizio.
* *list* di tutti i nomi di servizi disponibili.
* *lookup* di un servizio in base al nome.
# Approfondimenti