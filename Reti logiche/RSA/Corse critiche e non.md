---
subject: reti logiche
type: definizione
---
Nel caso in cui RSA debba cambiare stato e la distanza di bit tra le due codifiche sia maggiore di 1 è possibile che i bit singoli vengano cambiati in istanti diversi calcolando così degli stati intermedi diversi tra quello presente e futuro trovandosi così in una situazione di *corsa*.
* Una corsa è critica se si possono raggiungere stabilità diverse.
* Una corsa non è critica se si raggiunge sempre la stabilità prevista generando quindi una transizione multipla.
Perciò se le corse non critiche portano sempre alla stessa uscita durante la transizione multipla non rappresenta un problema per l'RSA.
Esistono alcune regole utili per prevenire eventuali corse critiche.
1. In eventuali colonne con una singola stabilità si inserisce lo stato stabile al posto delle celle di indifferenza.
2. Per le colonne con più stabilità si traccia in [[Grafo delle adiacenze]].
3. Si cerca di risolvere eventuali corse con transizioni multiple.
4. Se non si riesce si aumentano i bit di stato e si ripete dal punto due.