> [!definition] Segnale PAM aleatorio
> Se l'andamento nel tempo del segnale è dato da un [[Processo stocastico|processo stocastico]], allora il segnale è detto aleatorio, nel caso di un segnale PAM il segnale aleatorio è quello della [[Serie temporale|serie temporale]].

> [!definition] Autocorrelazione statistica
> Definiamo l'autocorrelazione statistica come il valore atteso del prodotto dei valori di distanza $k$ fra di loro
> $$
> E[a_n^\dagger a_{n+k}]
> $$
> supponendo che la serie sia stazionaria, cioè
> $$
> E[a_{n+k}]=E[a_{n+j}]
> $$
>  la probabilità della coppia è indipendente dalla posizione $n$ delle due variabili, ma solo dalla loro distanza, perciò definiamo
> $$
> c_{\text{stat},k}=E[a_n^\dagger a_{n+k}]=\sum_{i=1}^{l}\sum_{j=1}^{l}a_i^\dagger a_lP(a_i,a_l,k)
> $$
> dato che le due variabili $a_n$ e $a_{n+k}$ sono [[Eventi indipendenti|indipendenti]] si ha
> $$
> c_{\text{stat,k}}=E[a_n^\dagger a_{n+k}]=E[a_n^\dagger]E[a_{n+k}]=E[a_n^\dagger]E[a_n]
> $$
> se invece $k=0$
> $$
> c_{\text{stat},0}=E[a_n^\dagger a_n]=E[|a_n|^2]
> $$
> che è definita come potenza statistica

> [!definition] Serie ergodica
> Se la serie aleatoria è sia stazionaria che a memoria finita si ha che $a_n$ e $a_{n+k}$ sono [[Eventi indipendenti|indipendenti]] per $k$ sufficientemente grande, allora i valori attesi coincidono con valori ottenuti dopo il processo stocastico quindi come valori misurati dall'esperimento. perciò
> $$
> c_{\text{stat},k}=c_k
> $