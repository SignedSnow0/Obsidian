> [!definition] Segnale PAM
> Un segnale PAM è ottenibile come convoluzione fra una [[Serie temporale|serie temporale]] e un impulso
> $$
> s=\{a_n\}*g=\sum_{n=-\infty}^{+\infty}a_ng(t-nT)
> $$

> [!definition] Spettro di potenza bilatero di un segnale PAM deterministico
> $$
> G_{s,\text{bil}}=\frac{|G|^2}{2\pi T}\left[c_0+2\sum_{k=1}^{+\infty}c_k\cos(k\omega T)\right]
> $$
> se i termini della [[Serie temporale|serie temporale]] sono [[Rappresentazione ortonormale di segnali|ortogonali]], allora
> $$
> G_{s,\text{bil}}=\frac{c_0}{2\pi T}|G|^2
> $$
>`\begin{proof}`
> Se invece l'energia non è finita, ma la potenza lo è studiamo dello spettro di potenza considerando la funzione di [[Funzioni di crosscorrelazione e autocorrelazione|autocorrelazione]] (supponendo $c_0=0$)
> $$
> \varphi_s=\frac{1}{T}\{c_k\}*\dot\varphi_g
> $$
> allora per il [[Teorema di Parseval generalizzato|teorema di Parseval]] sappiamo che
> $$
> G_{s,\text{bil}}=\frac{\mathcal{F}[\varphi_s]}{2\pi}=\frac{1}{2\pi}\mathcal{F}[\dot\varphi_g]\mathcal{F}[\{c_k\}]=\frac{|G|^2}{2\pi T}\sum_{k=-\infty}^{+\infty}c_k\e^{-jk\omega T}
> $$
> Ricordando che se la [[Serie temporale|serie]] è reale, la sua [[Segnali tempo-discreti|autocorrelazione]] è reale e pari, si ha
> $$
> \sum_{k=-\infty}^{+\infty}c_k\e^{-jk\omega T}=c_0+2\sum_{k=1}^{+\infty}c_k\cos(k\omega T)
> $$
> ottenendo 
> $$
> G_{s,\text{bil}}=\frac{|G|^2}{2\pi T}\left[c_0+2\sum_{k=1}^{+\infty}c_k\cos(k\omega T)\right]
> $$
> infine, se i segnali della serie sono ortogonali l'autocorrelazione sarà nulla per ogni $k$ positivo, quindi
> $$
> G_{s,\text{bil}}=\frac{c_0}{2\pi T}|G|^2
> $$
> `\end{proof}`