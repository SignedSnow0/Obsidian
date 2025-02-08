I servizi di rete sono distinti in due categorie principali:
* Applicazioni **client/server** (ftp, telnet, ecc...).
* Applicazioni **distribuite** ([[Sistemi di Nomi#Domain Name System|DNS]], Mail, ecc...).

## Terminale remoto
Per gestire macchine di remoto è possibile utilizzare programmi come *telnet* o *ssh* (telnet con sicurezza) per accedere a terminali di altre macchine attraverso la rete. Il protocollo fornisce:
* **Comunicazione simmetrica** con funzioni distinte, complementari e differenziate.
* Gestione eterogeneità dei terminali con **terminale virtuale**.
* **Negoziazione** delle opzioni di collegamento.

Uno dei problemi principali del servizio è quello della gestione dei diversi terminali che possono differire per esempio per charset o dimensione. Per risolvere il problema si definisce un unico terminale standard chiamato **terminale virtuale**, allora il client trasformerà i propri dati nello standard e il server passerà dallo standard al proprio per l'esecuzione dei comandi.
* Allo startup **NVT** prevede caratteri da 7 bit ASCII passati un byte alla volta.
* ASCII prevede caratteri speciali che non vengono stampati, chiamati **caratteri di controllo**, questi permettono l'esecuzione di comandi speciali sia in fase di esecuzione che in fase di negoziazione.
* La fase di negoziazione è svolta come prima cosa durante la creazione della connessione, nel processo il client richiede una specifica al server, che risponderà se la supporta o meno. La richiesta e risposta sono rappresentate con i caratteri di controllo.
## Trasferimento File
Per il trasferimento file esistono due servizi principali: *FTP* su TCP o *Trivial FTP* su UDP, entrambi forniscono i seguenti strumenti:
* Controllo di identità per l'accesso sulla macchina remota.
* Esecuzione di alcuni programmi sul server (ls, cd, ecc...).
* Trasferimento files binari e di testo (singoli e multipli).

La comunicazione tra i terminali è effettuata con NVT come per telnet, inoltre le operazioni sono tutte sincrone con messaggi di risposta di tre cifre, simili alle risposte web.
Il server è composto da un processo padre che si occupa della creazione della connessione che viene poi passata ad un processo figlio per l'interazione con il client, che a sua volta può creare altri processi per il trasferimento file.
La connessione per il trasferimento dati è effettuata in una seconda socket con porta negoziata fra i due, il protocollo è diverso se il cliente è considerato attivo o passivo:
* Se il client è attivo, il server fa una listen ed è il client a dover fare la connect per stabilire la connessione.
* Se il client è passivo, il server fa la connect mentre il client è in listen.

Il caso con client passivo è più facile da implementare dato che il server una volta che riceve la porta della connessione dal client sa che la listen è già stata fatta e non si presenteranno problemi di rendez-vous.
## Posta elettronica
I servizi di posta elettronica sono divisi agenti di due categorie:
* User Agents: sono la parte del servizio finale, che interagisce con gli utenti.
* Message Transfer Agents: sono i nodi posti tra gli utenti, si occupano del trasferimento del messaggio tra il mittente e i possibili destinatari.

Il servizio di posta elettronica è asincrono, infatti il mittente non attende che il messaggio sia arrivato al destinatario, infatti sotto il messaggio è solamente al primo MTA di una possibile lunga catena che si occupa in maniera collaborativa della distribuzione della mail.
Il messaggio è diviso in header e body, l'header contiene informazioni di metalivello come mittente, destinatari, data di creazione, ecc..., il body contiene il testo del messaggio che con il tempo si è evoluto ed ora può essere composto da contenuti diversi secondo i formati MIME come immagini o files.
I nomi del servizio mail è composto da una parte specifica per utente chiamata mailbox seguita da un nome di dominio risolta nell'indirizzo IP del server finale, inoltre sono supportati alias e gruppi di mailing sotto nomi simbolici.
Il trasporto stesso della mail è diviso in due protocolli differenti:
* POP o IMAP per lo scambio tra MTA e UA
* SMTP per lo stambio tra due MTA composto da comandi di testo e risposte a tre cifre simili al web, trasferimento a transazioni con rollback in caso di errore.


