---
subject: fondamenti di telecomunicazioni
---
Nel caso particolare di un segnale $x$ periodico e reale si ha che i coefficienti $c_n$ della [[Forma esponenziale di segnali complessi|serie di Fourier]] dispongono di simmetria hermitiana
> [!definition] Simmetria hermitiana
> $$
> c_{n}=c_n^{\dagger}
> $$
> perciò le coppie di coefficienti avranno uguale ampiezza e fase opposta:
> $$
> |c_{n}|=|c_{-n}|
> $$
> $$
> \angle c_n=-\angle c_{-n}
> $$

Sfruttando quindi la simmetria hermitiana è possibile semplificare la [[Forma esponenziale di segnali complessi|rappresentazione generale]]
$$
x=\sum_{n=-\infty}^{-1}c_n\e^{jn\omega_0t}+c_0+\sum_{n=1}^{+\infty}c_n\e^{jn\omega_0t}=
$$
$$
=\sum_{n=1}^{+\infty}c_{-n}\e^{-jn\omega_0t}+c_0+\sum_{n=1}^{+\infty}c_n\e^{jn\omega_0t}=
$$

> [!definition] Rappresentazione con fasori
> $$
> x=c_0+\sum_{n=1}^{+\infty}2\Re\{c_n\e^{jn\omega_0t}\}
> $$

Definendo gli [[Spettri di ampiezza e fase bilateri|spettri di ampiezza e fase monolateri]] come
$$
\begin{cases}A_0=c_0\\ A_n=2|c_n|\end{cases}
$$
$$
\phi_n=-\angle c_n
$$
si ha la forma in soli coseni e fase iniziale
> [!definition] Rappresentazione con coseno e fase
> $$
> x=A_0+\sum_{n=1}^{+\infty}A_n\cos(n\omega_0t-\phi_n)
> $$

Infine definendo i coefficienti $a_n,b_n$
$$
a_n=\begin{cases}2c_0&n=0\\\Re\{2c_n\}&n>0\end{cases}
$$
$$
b_n=-\Im\{2c_n\}\quad n>0
$$
si ottiene la forma in termini di seni e coseni
> [!definition] Rappresentazione con seni e coseni
> $$
> x=\frac{1}{2}a_0+\sum_{n=1}^{+\infty}a_n\cos(n\omega_0t)+\sum_{n=1}^{+\infty}b_n\sin(n\omega_0t)
> $$

Infine ricordiamo che i coefficienti $a_n,b_n$ sono ricavabili senza passare per i coefficienti $c_n$
> [!lemma]
> $$
> a_n=\frac{2}{T}\int_{-\frac{T}{2}}^{\frac{T}{2}}dtx\cos(n\omega_0t)\quad n\ge0
> $$

> [!lemma]
> $$
> b_n=\frac{2}{T}\int_{-\frac{T}{2}}^{\frac{T}{2}}dtx\sin(n\omega_0t)\quad n>0
> $$