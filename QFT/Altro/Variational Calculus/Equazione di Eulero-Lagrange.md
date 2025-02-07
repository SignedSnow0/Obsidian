[Video](https://youtu.be/VCHFCXgYdvY?si=EHoa0j1Ze7NOVO3J)
L'equazione di Eulero-Lagrange vuole minimizzare la Lagrangiana, vogliamo quindi trovare una seconda funzione che minimizza $\mathcal{L}$ in ogni punto del percorso, abbiamo allora un problema di calcolo delle variazioni.
$$
\mathcal{S}=\int_{x_1}^{x_2}\mathcal{L}(t,q,\dot{q})dx
$$
allora $\mathcal{S}$ è un funzionale o funzione di funzione.

---
Parametrizziamo le funzioni possibili tra i punti $x_1$ e $x_2$:
Abbiamo la funzione $y(x)$ che è la soluzione del nostro problema, e poi abbiamo un insieme di infinite funzioni che deviano dalla nostra soluzione $y(x)$ per un valore $\eta(x)$ e una proporzione $\epsilon$
allora tutti i generali percorsi sono
$$
\bar{y}(x)=y(x)+\epsilon\eta(x)
$$
in maniera analoga al differenziale di una funzione $x+dx$, $\epsilon\eta(x)$ è chiamata la variazione del funzionale.
Inoltre, dato che ogni percorso deve iniziare in $x_1$ e terminare in $x_2$ si ha che
$$
\eta(x_1)=\eta(x_2)=0\quad\forall\eta
$$
Consideriamo allora
$$
I=\int_{x_1}^{x_2}F[x,y,y']dx
$$
allora, come per i punti di estremo di una funzione, se $y$ è un percorso di estremo, allora deve essere un punto stazionario, quindi $I=0$.
Consideriamo le funzioni generali $\bar{y}$, per il principio precedente $y$ è estremo, quindi costante, $\eta$ è una funzione che una volta scelta rimane costante, allora la variazione di $I$ è solamente in $\epsilon$, quindi
$$
\frac{\partial I}{\partial\epsilon}=\frac{dI}{d\epsilon}
$$
perciò il percorso ideale sarà
$$
\evals{\frac{dI}{d\epsilon}}{\epsilon=0}=\evals{\frac{d}{d\epsilon}}{\epsilon=0}\int_{x_1}^{x^2}F[x,\bar{y},\bar{y}']dx=0
$$
che equivale a 
$$
\int_{x_1}^{x^2}\evals{\frac{d}{d\epsilon}F[x,\bar{y},\bar{y}']}{\epsilon=0}dx=0
$$
espandiamo la derivata 
$$
\int_{x_1}^{x_2}\evals{\left(\frac{\partial F}{\partial\epsilon}\frac{\partial x}{\partial \epsilon}+\frac{\partial F}{\partial \bar{y}}\frac{\partial\bar{y}}{\partial \epsilon}+\frac{\partial F}{\partial\bar{y}'}\frac{\partial\bar{y}'}{\partial\epsilon}\right)}{\epsilon=0}dx=0
$$
ricordando che $\bar{y}=y+\epsilon\eta$ e quindi $\frac{\partial\bar{y}}{\partial\epsilon}=\eta$ e $\frac{\partial\bar{y}'}{\partial\epsilon}=\eta'$ si ha
$$
\int_{x_1}^{x_2}\evals{\left(\frac{\partial F}{\partial\bar{y}}\eta+\frac{\partial F}{\partial\bar{y}'}\eta'\right)}{\epsilon=0}dx=0
$$
ricordando che per $\epsilon\to0\implies\bar{y}\to y,\ \bar{y}'\to y'$
$$
\int_{x_1}^{x^2}\left(\frac{\partial F}{\partial y}\eta+\frac{\partial F}{\partial y'}\eta'\right)dx=0
$$
questa formula rappresenta la prima variazione i forma debole o variazionale, si dive debole perchè c'è $\eta'$ e non $\eta$.
Allora per integrazione per parti si ha
$$
\int_{x_1}^{x_2}\frac{\partial F}{\partial y'}\eta'dx=\eval{\frac{\partial F}{\partial y'}\eta}{x_1}{x_2}-\int_{x_1}^{x^2}\frac{d}{dx}\left(\frac{\partial F}{\partial y'}\right)\eta dx
$$
ma ricordando la restrizione del percorso agli estremi si ha che 
$$
\eval{\frac{\partial F}{\partial y'}\eta}{x_1}{x_2}=0
$$
perciò reinserendo il risultato nella formula iniziale
$$
\int_{x_1}^{x_2}\left(\frac{\partial F}{\partial y}-\frac{d}{dx}\left(\frac{\partial F}{\partial y'}\right)\right)\eta dx=0
$$
ottenendo così la prima variazione in forma forte o differenziale.
Ora, per  il lemma fondamentale del calcolo delle variazioni si ha che
$$
\frac{\partial F}{\partial y}-\frac{d}{dx}\left(\frac{\partial F}{\partial y'}\right)=0
$$
infine con un po di sostituzioni si ottiene l'equazione di Eulero-Lagrange
$$
\frac{\partial\mathcal{L}}{\partial q}=\frac{d}{dt}\left(\frac{\partial\mathcal{L}}{\partial\dot{q}}\right)
$$
---
### Derivazione con operatore variazionale $\delta$
[Video](https://youtu.be/vqDHO2eKXcs?si=FS8hpKMhpch-ag5O)