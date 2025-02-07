## Definizione di ket
In meccanica quantistica una particella è un vettore in uno spazio vettoriale
> [!definition] Spazio vettoriale
> Un insieme $V$ è uno **spazio vettoriale** se per ogni vettore $u,v,w$ e scalare $a,b$ si ha:
> 1. $$
> u+v\in V
> $$
> 2. $$
au\in V
> $$
> 3. $$
u+(v+w)=(u-v)+w
> $$
> 4. $$
u+v=v+u
> $$
> 5. $$
\exists\,0\in V
> $$
> 6. $$
\exists\,-u\in V
> $$
> 7. $$
a(bu)=(ab)u
> $$
> 8. $$
1u=u
> $$
> 9. $$
a(u+v)=au+av
> $$
> 10. $$
(a+b)u=au+bu
> $$

Un vettore allora rappresenta uno stato quantistico, valore che contiene tutte le informazioni della particella per ogni momento nel tempo, il simbolo utilizzato è
$$
\ket{\psi}
$$
Per esempio, se vogliamo rappresentare i possibili valori di energia $E_k$ di un onda $\psi$, avremo una superposizione di tutti i possibili stati di energia che è rappresentata da una combinazione lineare
$$
\ket{\psi}=c_1\ket{E_1}+\dots+c_n\ket{E_n}
$$
dove i coefficienti $c_k$ indicano la probabilità di avere la particella in quel particolare stato.
Per rappresentare valori continui abbiamo bisogno di una somma infinita su elementi continui: un integrale
$$
\ket{\psi}=\int dx\;c(x)\ket{x}
$$
dove $dx$ indica che l'integrale è effettuato sulla posizione, il ket $\ket{x}$ contiene le informazioni sulla posizione $x$ che rappresentano, e $c(x)$ è la probabilità di avere il ket specifico.
Notiamo che allora la combinazione lineare e l'integrale sono completamente analoghi.

---
## Spazio vettoriale infinito e spazio di Hilbert
Per rappresentare lo stato di una particella abbiamo detto che essa è una combinazione lineare di tutti i valori possibili, ma questi valori potrebbero essere infiniti, perciò lo spazio vettoriale potrebbe avere dimensione infinita.
$$
\ket{\psi}=\sum_{i=1}^{\infty}c_i\ket{E_i}
$$
Ciò potrebbe portare a problemi:
Consideriamo lo spazio vettoriale dei polinomi, allora una base sono tutte le potenze di $x$
$$
\{x^0,\dots,x^n\}
$$
prendiamo ora una funzione non polinomiale $e^x$, allora esiste una serie di Taylor tale che
$$
e^x=\sum_{i=1}^{\infty}\frac{x^i}{i!}
$$
abbiamo quindi che una combinazione lineare di infiniti polinomi porta a un elemento non polinomiale, rompendo la condizione di chiusura della definizione di spazio vettoriale.
> [!definition] Spazio di Hilbert
> Definiamo uno **spazio di Hilbert** come **uno spazio vettoriale con un prodotto interno che è Cauchy complete**, cioè con un prodotto scalare dove ogni serie convergente di elementi dello spazio risulta in un elemento dello spazio stesso.
>$$
\mathcal{H}
>$$
---
## Prodotto interno
In linea di massima il prodotto interno è una generalizzazione del prodotto scalare, nella forma rigorosa è una funzione da due elementi dello spazio vettoriale a un numero
$$
\braket{\psi}{\phi}=c
$$
Proprietà.
1. Il prodotto interno è lineare per il ket
$$
\braket{\psi}{\phi+\zeta}=\braket{\psi}{\phi}+\braket{\psi}{\zeta}
$$
$$
\braket{\phi}{a\psi}=a\braket{\phi}{\psi}
$$
2. È anticommutativo
$$
\braket{\psi}{\phi}=\braket{\phi}{\psi}^*
$$
3. È definito positivo
$$
\braket{\psi}{\psi}\ge0
$$
$$
\braket{\psi}{\psi}=0\iff\ket{\psi}=0
$$
4. È antilineare per il bra
$$
\braket{a\psi+b\zeta}{\phi}=a^*\braket{\psi}{\phi}+b^*\braket{\zeta}{\phi}
$$

Definiamo allora una base ortonormale per lo spazio vettoriale
$$
\{E_n\}:\quad\braket{E_i}{E_j}=\delta_{ij}
$$
dove $\delta_{ij}$ è il delta di Kroneker
Allora possiamo facilmente trovare la probabilità di uno stato
> [!theorem]
> $$
\braket{E_j}{\psi}=c_j
> $$
> `\begin{proof}`
Esprimiamo $\ket\psi$ come combinazione lineare
> $$
\ket\psi=\sum_ic_i\ket{E_i}
> $$
 Facciamo il prodotto interno con l'elemento della base corrispondente al coefficiente
 cercato
> $$
\braket{E_j}{\psi}=\bra{E_j}\left(\sum_ic_i\ket{E_i}\right)
> $$
Per la linearità del prodotto interno
> $$
\braket{E_j}{\psi}=\sum_ic_i\braket{E_j}{E_i}
> $$
Dato che la base è ortonormale
> $$
\braket{E_j}{\psi}=\sum_ic_i\delta{ji}=c_j
> $$ 
> `\end{proof}`

> [!theorem]
> $$
\displaystyle\braket{\psi}{\phi}=\sum_ia_i^*b_i
> $$
> `\begin{proof}`
Espandiamo i vettori nelle loro basi
> $$
\braket{\psi}{\phi}=\left(\sum_i\bra{a_iE_i}\right)\left(\sum_j\ket{b_jE_j}\right)=\sum_i\sum_j\braket{a_iE_i}{b_jE_j}
> $$
>Per linearità e antilinearità
> $$
\braket{\psi}{\phi}=\sum_i\sum_ja_i^*b_j\braket{E_i}{E_j}
> $$
Dato che la base è ortonormale
> $$
\braket{\psi}{\phi}=\sum_i\sum_ja_i^*b_j\delta_{ij}=\sum_ia_i^*b_i
> $$
> `\end{proof}`

Notiamo che se $a,b$ sono numeri reali allora $\braket{\psi}{\phi}$ è il prodotto scalare, perciò otteniamo che il prodotto scalare è un caso particolare del prodotto interno in una base ortonormale.

---
## Delta di Dirac e prodotto interno continuo
Assumiamo di avere una base ortonormale continua, allora dalla [[#Definizione di ket|definizione di ket]] abbiamo che
$$
\ket{\psi}=\int dx\;c(x)\ket{x}
$$
ma come per il [[#Prodotto interno|prodotto interno]] discreto vogliamo riuscire ad ottenere una particolare probabilità di una soluzione dall'onda
$$
c(x_0)\approx\int dx\;c(x)\braket{x_0}{x}
$$
la soluzione è quella di usare una particolare funzione chiamata delta di Dirac
$$
c(x_0)=\int dx\;c(x)\delta(x_0-x)
$$
> [!definition] Delta di Dirac
> Il delta di Dirac è una qualsiasi funzione che soddisfa le seguenti:
> 1. $$
\delta(x)=\begin{cases}\infty&x=0\\0&x\ne0\end{cases}
> $$
> 2. $$
\int dx\;\delta(x)=1
> $$
> 
> Un ulteriore definizione di delta di Dirac più pratica è la seguente:
> Il delta di Dirac è una funzione $\delta$ che soddisfa la seguente proprietà
> $$
f(x_0)=\int_\mathbb{R} dx\;f(x)\delta(x_0-x)
> $$

Vediamo allora che
$$
\int dx\;c(x)\delta(x_0-x)=\begin{cases}0&x\ne x_0\\\displaystyle\int dx\;c(x_0)&x=x_0\end{cases}=c(x_0)\int dx=c(x_0)
$$
> [!example] Distribuzione normale
> Un esempio di funzione che soddisfa il delta di Dirac è la distribuzione gaussiana per una varianza che tende a 0
> $$
\lim_{a\to0}\frac{1}{a\sqrt{2\pi}}e^{-\frac{x^2}{2a^2}}
> $$
Tornando ora all problema originario abbiamo che
$$
\braket{x_i}{x_j}\approx\delta(x_i-x_j)
$$
prediamo quindi il prodotto di due vettori
$$
\braket{\psi}{\phi}
$$
dato che la loro base è continua, la loro rappresentazione diventa
$$
\left(\int dx\;\psi(x)\bra{x}\right)\left(\int dy\;\phi(y)\ket{y}\right)
$$
per le proprietà del [[#Prodotto interno|prodotto interno]]
$$
\iint dxdy\;\psi(x)^*\phi(y)\braket{x}{y}=\iint dxdy\;\psi(x)^*\phi(y)\delta(x-y)
$$
per la proprietà del delta di Dirac
$$
\braket{\psi}{\phi}=\int dx\;\psi(x)^*\phi(x)
$$
che è la definizione di prodotto interno per funzioni continue.

---
## Definizione di bra
Iniziamo definendo un funzionale lineare
> [!definition] Funzionale lineare
> Un funzionale lineare è una trasformazione lineare che da un elemento dello spazio vettoriale restituisce uno scalare reale o complesso

Cerchiamo ora di capire come è fatta la matrice che rappresenta i funzionali lineari:
Sappiamo che un funzionale $L:\mathbb{R}^n\to\mathbb{R}$, perciò la matrice sarà $1\times n$, perciò è un vettore girato.
Inoltre l'insieme delle matrici riga formano uno spazio vettoriale chiamato spazio duale di $V$ indicato con
$$
V^*
$$
perciò ogni funzionale lineare $L$ per lo spazio $V$ è in $V^*$.
Notiamo ora che ogni volta che vogliamo estrarre un risultato dalla particella $\ket{\psi}$ stiamo estraendo uno scalare da un vettore, quindi un funzionale lineare sarà sicuramente coinvolto, allora assegnando il simbolo di bra all'operatore lineare 
$$
\bra{\phi}\in\mathcal{H}^*
$$
si ha che
$$
\bra{\phi}\ket{\psi}=c
$$
Notiamo che $\bra{\phi}\ket{\psi}=c$ ricorda il [[#Prodotto interno|prodotto interno]], infatti moltiplicare una matrice riga con un vettore risulta nel prodotto scalare.
> [!theorem] Teorema di Rappresentazione di Riesz
> Per ogni funzionale lineare $L_\phi$, l'azione di $L_\phi$ è equivalente a fare il prodotto interno con un vettore $\vec{\phi}$
> $$
L_\phi\vec{v}=\braket{\vec{\phi}}{\vec{v}}
> $$

Con questo teorema possiamo dimostrare che
$$
\bra{\phi}\ket{\psi}=\braket{\phi}{\psi}
$$
Facciamo allora un esempio dell'importanza di questa notazione:
> [!exercise] 
> Data una funzione $\ket{\psi}=\sum c_i\ket{A_i}$, ricordiamo che $c_i=\braket{A_i}{\psi}$, allora
> $$
\ket\psi=\sum\braket{A_i}{\psi}\ket{A_i}
> $$
> usando quanto abbiamo visto 
> $$
\ket\psi=\sum\ket{A_i}\braket{A_i}{\psi}=\sum\ket{A_i}\bra{A_i}\ket{\psi}=\left(\sum\braket{A_i}{A_i}\right)\ket\psi
> $$
> allora avremo che 
> $$
\sum\ket{A_i}\bra{A_i}=\hat{I}
> $$
---
## Osservabili e operatori
> [!definition] Osservabile
> In fisica quantistica un **osservabile** è una qualsiasi quantità che possiamo misurare.

> [!definition] Operatore lineare
> Un **operatore lineare** è una mappa su uno spazio vettoriale che lo mantiene lineare, cioè:
> 1. $$
\hat{M}(\ket\psi+\ket\phi)=\hat{M}\ket\psi+\hat{M}\ket\phi\quad\forall\psi,\phi\in V
> $$
> 2. $$
\hat{M}(\lambda\ket\psi)=\lambda\hat{M}\ket\psi\quad\forall\psi\in V,\lambda\in\mathbb{R}
> $$

Presupponiamo ora di fare un esperimento per determinare per esempio il momento angolare di una particella, allora si avrà che essa ha un valore specifico $L_1$
$$
L_1=x\ Nms
$$
e la funzione associata dopo la misurazione avrà un unico ket che la definirà con probabilità assoluta chiamato **stato definito**
$$
\ket\psi=\ket{L_1}
$$
Allora possiamo dedurre che per ogni osservabile $\hat{E}$ che vogliamo rappresentare dobbiamo trovare ogni possibile valore $E_k$ che rappresenta un autovalore e ogni possibile stato associato $\ket{E_k}$ che rappresenta un autovettore o in questo contesto un autostato.
Allora tornando alla definizione di particella come superposizione di possibili valori, ora sappiamo che questi valori sono gli autostati della particella
$$
\ket\psi=c_1\ket{E_1}+c_2\ket{E_2}+\dots
$$
Possiamo allora derivare alcune fondamentali proprietà degli operatori lineari:
1. Ogni osservabile deve avere autovalori reali
2. Gli autostati di un osservabile devono estendere tutto lo spazio vettoriale, quindi ogni particella può essere descritta come combinazione lineare degli autostati
$$
\ket\psi=\sum c_i\ket{E_i}
$$
3. Dato che per ogni misurazione sicuri di ottenere solo un autovalore al 100%, gli autostati devono essere ortogonali fra loro.

Allora dalle proprietà 2 e 3 abbiamo che gli autostati di un osservabile formano una base ortonormale di autovettori.

---
# Regola di Born