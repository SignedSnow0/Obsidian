> [!definition] Sistema trifase
> Un sistema di distribuzione trifase è composto da 3 cavi che portano tensioni elettriche di uguale modulo e ognuna sfasata di $120\degree$ dalla prossima.
> Questo sistema porta ai seguenti vantaggi:
> * I costi di costruzione sono minori. (non c'è un cavo di neutro)
> * Ci sono minori perdite di potenza lungo la linea.
> * Ottengo un campo magnetico variante nel tempo.

> [!definition] Sfasamento nel sistema trifase
> Sappiamo che: 
> 1. Le tensioni di ogni fase sono sinusoidali isofrequenziali.
> 2. Le tensioni hanno lo stesso valore di picco.
> 3. La somma delle tre fasi è nulla.
>
> Abbiamo allora che
> $$
> V\e^{\varphi_{1,2}}+V\e^{\varphi_{2,3}}+V\e^{\varphi_{3,1}}=0
> $$
> $$
> \e^{\varphi_{1,2}}+\e^{\varphi_{2,3}}+\e^{\varphi_{3,1}}=0
> $$
> $$
> \e^{\varphi_{1,2}}+\e^{\varphi_{2,3}}+\e^{\varphi_{3,1}}+1=1
> $$
> $$
> \varphi_{1,2}+\varphi_{2,3}+\varphi_{3,1}=\ln(1)=0
> $$
> allora abbiamo che la somma delle tre fasi deve essere pari ad un periodo, cioè
> $$
> \varphi_{1,2}=0,\ \varphi_{2,3}=120\degree,\ \varphi_{3,1}=-120\degree
> $$

> [!definition] Modello di generatore trifase
> Modelliamo un generatore trifase come tre generatori separati in carico a stella:
> Applicando 3 [[Leggi di Kirchhoff|LKT]] abbiamo il seguente sistema:
> $$
> \begin{cases}\underline{E}_{2,O}-\underline{V}_{1,2}-\underline{E}_{1,O}=0\\\underline{E}_{3,O}-\underline{V}_{2,3}-\underline{E}_{2,O}=0\\\underline{E}_{1,O}-\underline{V}_{3,1}-\underline{E}_{3,O}=0\end{cases}
> $$
> $$
> \begin{cases}\underline{V}_{1,2}=\underline{E}_{1,O}-\underline{E}_{2,O}\\\underline{V}_{2,3}=\underline{E}_{2,O}-\underline{E}_{3,O}\\\underline{V}_{3,1}=\underline{E}_{3,O}-\underline{E}_{1,O}\end{cases}
> $$
> con un pò di geometria si ottiene allora che
> $$
> \underline{V}=\sqrt{3}\underline{E}
> $$

> [!definition] Bilanciamento dei carichi
> In un sistema reali i carichi sulle 3 fasi possono essere indipendenti l'uno dall'altro, ciò porta ad potenziale sul nodo comuno non nullo.
> Allora si hanno delle tensioni sugli utilizzatori pari a 
> $$
> \begin{cases}\underline{E}_{1,O}'=\underline{E}_{1,O}-\underline{V}_{O,O'}\\\underline{E}_{2,O}'=\underline{E}_{2,O}-\underline{V}_{O,O'}\\\underline{E}_{3,O}'=\underline{E}_{3,O}-\underline{V}_{O,O'}\end{cases}
> $$
> esprimendo le correnti di $\underline{E}'$ e applicando l'[[Leggi di Kirchhoff|LKC]] sul nodo $O'$ si ha
> $$
> \frac{\underline{E}_{1,O}-\underline{V}_{O,O'}}{\underline{Z}_1}+\frac{\underline{E}_{2,O}-\underline{V}_{O,O'}}{\underline{Z}_2}+\frac{\underline{E}_{3,O}-\underline{V}_{O,O'}}{\underline{Z}_3}=\underline{0}
> $$
> allora
> $$
> \underline{V}_{O,O'}=\frac{\frac{\underline{E}_{1,O}}{\underline{Z}_1}+\frac{\underline{E}_{2,O}}{\underline{Z}_2}+\frac{\underline{E}_{3,O}}{\underline{Z}_3}}{\frac{1}{\underline{Z}_1}+\frac{1}{\underline{Z}_2}+\frac{1}{\underline{Z}_3}}
> $$
> allora se il carico è equilibrato, cioè $\underline{Z}_1=\underline{Z}_2=\underline{Z}_3$ si ha
> $$
> \underline{V}_{O,O'}=\underline{E}_{1,O}+\underline{E}_{2,O}+\underline{E}_{3,O}=0
> $$
> altrimenti si aggiunge un cavo di corto fra $O$ e $O'$ per assicurare $\underline{V}_{O,O'}=\underline{0}$, in questo cavo si avrà una corrente $\underline{I}_N$ pari a
> $$
> \underline{I}_{N}=\frac{\underline{E}_{1,O}}{\underline{Z}_1}+\frac{\underline{E}_{2,O}}{\underline{Z}_2}+\frac{\underline{E}_{3,O}}{\underline{Z}_3}
> $$