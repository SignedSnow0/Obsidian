I Sistemi di Nomi sono servizi distribuiti fondamentali che forniscono la locazione fisica di un nodo in base ad un nome logico, permettendo il **binding dinamico** di applicazioni terze.
I sistemi di nomi *in the large* sono a loro volta distribuiti e divisi in più agenti per:
* Partizionare la capacità di servizio.
* Replicare il servizio.

Questa architettura divisa permette la risoluzione di un nome in tempi accettabili, mantenendo la dinamica possibilità di aggiungere nomi o interi nodi, e aggiungere QoS con replicazione e caching su ogni livello.
## Domain Name System
Il DNS è un sistema di nomi che permette di ottenere un indirizzo IP da un nome logico (di dominio), consiste in un albero percorso in direzione inversa del nome di dominio fornito dove di solito ogni ramo dell'albero rappresenta un nodo fisico del sistema DNS.
* Un nome DNS è al massimo di 255 caratteri con massimo 63 per parte, tutti case insensitive.
* Il client fa richieste attraverso un agente intermedio locale chiamato **name resolver**.
* Se la query è di tipo **iterativo** ad ogni risposta del server DNS, se il server non è di competenza la risposta indica il prossimo server nella rete che potrebbe contenere la risposta, il name resolver inoltrerà poi una richiesta al secondo server, fino all'ottenimento del nome.
* Se la query è di tipo **ricorsivo** il server a cui è stata effettuata la query si prende carico di inoltrare la domanda fino al server di competenza, la risposta sale poi la coda fino all'arrivo al name resolver.
* Ogni agente del sistema fa utilizzo di **caching** per ottimizzare i tempi di risposta e minimizzare il numero di query secondo il principio di località.
* I sistemi unix prima di richiedere una query fanno lookup del nome su un file in **/etc/hosts**.
* Le richieste DNS sono effettuate con protocollo UDP sulla porta 53, con eventuale supporto a TCP dopo un messaggio di eccezione.
* Alcuni server, ma non tutti permettono query inverse.

I record DNS contengono ulteriori informazioni oltre all'indirizzo IP:
* Nome di dominio
* Time To Live
* Classe (protocollo utilizzato)
* Tipo (IP, Name Server, Pointer, ecc...)
* Valore
## X500
X500 è un protocollo OSI di **direttorio**, in poche parole ogni elemento del servizio è composto da un insieme di attributi.
* I nodi sono situati su un **albero con interconnessioni** (grafo?) chiamato **Directory Information Tree**.
* Ogni nodo è costituito da **attributi tipizzati**.
* Gli attributi sono assegnati in maniera **gerarchica**, i nodi figli ereditano tutti gli attributi del padre.
* Le operazioni sono protette da **autorizzazione**.
* I nodi sono **replicati** per garantire QoS.
* Le operazioni più frequenti e per questo più ottimizzate sono le **query** sugli attributi delle directory, sono supportati **aggiornamenti** e **inserimento** di valori.
* Le operazioni di ricerca sono svolte in **parallelo**.
* Il nome assoluto di un nodo si chiama **Distinguished Name**, le relativizzazioni si chiamano **Relative Distinguished Name**.