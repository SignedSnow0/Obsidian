Per garantire il funzionamento di più processi il sistema operativo deve permettere:
* Allocazione / Deallocazione della memoria.
* Protezione delle aree di memoria da altri processi.
* Gestire casi dove la memoria richiesta è superiore a quella disponibile.

Inoltre un programma scritto fa riferimento allo stack attraverso indirizzi logici, dove lo 0 è il primo byte del programma, mentre nella realtà il programma non parte dal primo byte dello spazio di indirizzamento, perciò avviene un meccanismo chiamato binding.

> [!definition] Binding
> Il binding è meccanismo attraverso il sistema operativo trasla gli indirizzi logici del codice negli indirizzi veri dello spazio di indirizzamento, di solito è effettuato all'avvio del processo per permettere dinamicismo.
---
## Paginazione
Una prima soluzione per il caricamento in memoria di un processo è quella di creare una partizione della ram dove verrà poi allocato il programma:
* se queste partizioni sono di dimensione fissa il SO potrà caricare solo N programmi alla volta
* se invece le partizioni sono di dimensione variabile in generale si possono caricare più programmi, generando così il problema della frammentazione dello stack.

In entrambi i casi, per ogni processo vengono assegnati due registri *RR* (Registro di Rilocazione) e *RL* (Registro Limite) che indicano il primo e ultimo indirizzo fisico disponibile che vengono utilizzati per errori di segmentazione.

Una seconda soluzione più moderna è quella dell'allocazione non contigua attraverso il meccanismo della paginazione.
> [!definition] Paginazione
> Una pagina della memoria è un segmento di dimensioni fisse sulla quale viene allocata una parte del processo finché non è completamente caricato.
> * Le pagine di un singolo processo possono essere non contigue, mitigando il problema della frammentazione.
> * È possibile se necessario spostare queste pagine in memoria secondaria per fare spazio ad altri processi (memoria virtuale).

Utilizzando questo meccanismo un indirizzo logico è diviso in due parti
* *p* indica l'indice della **pagina** del processo
* *d* indica l'**offset** all'interno della pagina

Questo meccanismo è talmente utilizzato che per velocizzare la traslazione logico-fisica degli indirizzi le cpu moderne hanno strutture hardware dedicate:
* Il **PageTableBaseRegister** è una tabella nella memoria primaria che contiene le posizioni fisiche delle pagine nello spazio di indirizzamento.
* Il **TranslationLook-asideBuffer** è una cache che contiene le entry più utilizzate del PTBR.

Inoltre per sapere se una pagina contiene dati realmente allocati da un processo ogni pagina ha 
* un **bit di validità** per sapere se è stata allocata
* una seconda tabella chiamata **PageTableLenghtRegister** che indica la lunghezza dei dati validi dentro una pagina
* Un **bit di protezione** che indica la modalità di accesso (read-only, ...)
---
## Segmentazione
> [!definition] Segmentazione
> La segmentazione è una tecnica di allocazione della memoria basata della divisione logica dei segmenti del programma, in generale sono:
> * Dati (variabili const e static)
> * Codice 
> * Stack
> * Heap

Un indirizzo logico è diviso un due parti, una che individua il **segmento** e una per l'**offset** all'interno del segmento.
Anche per questo metodo esiste supporto hardware con la **SegmentTableBaseRegister** e una cache per i record più usati.

--- 
## Memoria virtuale
> [!definition] Memoria virtuale
> La memoria virtuale è una tecnica di allocazione della memoria che permette di allocare solo in maniera parziale i processi nella memoria primaria per aumentare lo spazio disponibile.

Nella pratica ogni processo caricato è associato ad un segmento in memoria di massa dove verrà trasferito se necessario. Il componente del sistema operativo che si occupa di questo si chiama pager (singole pagine) o swapper (interi processi), di solito un metodo lazy.
Come per gli altri metodi esiste una tabella hardware chiamata **PageTableBaseRegister** con un bit che indica se la **pagina si trova in memoria primaria o meno**, se si vuole agire su una pagina che è in memoria di massa il sistema operativo genera una **page fault**.
Al ricevimento di una page fault il kernel:
1. Salva il contesto del processo attuale.
2. Verifica se il page fault è legale o illegale.
3. Se il page fault è illegale (segfault) il processo viene terminato.
4. Altrimenti copia la pagina in un frame libero, se non ci sono frame liberi ne sposta uno o più in memoria di massa.
5. Aggiorna la PTBR.
6. Ripristina il contesto del processo.

Se  alla generazione di un page fault non ci sono segmenti liberi ci troviamo in un caso di **sovrallocazione**, allora almeno un frame dovrà essere trasferito in memoria di massa, per scegliere quale pagina spostare ci sono diversi algoritmi:
* Esiste un bit chiamato **dirty bit** che indica se la pagina è stata modificata rispetto alla corrispondente in memoria di massa, se non è stata modificata lo swap non è necessario.
* LeastFrequentlyUsed
* FirstInFirstOut
* LeastRecentlyUsed
* Pre-paginazione consiste nel caricamento di più pagine alla volta (working set) in base al principio di **località spaziale** o **temporale** per ridurre la quantità di page faults. 