---
subject: fondamenti di telecomunicazioni
---
Un qualsiasi segnale è rappresentabile come [[Combinazione lineare|combinazione lineare]] di funzioni che ne compongono la [[Base ortonormale|base ortonormale]] dello [[Spazio vettoriale|spazio]].
Iniziamo definendo il [[Prodotto scalare|prodotto interno]] fra due segnali $x,y$ nell'intervallo $T$:
> [!definition] Prodotto interno fra segnali
> $$
> \langle x,y\rangle_T=\int_Tdtxy^\dagger
> $$

da questa definizione ricaviamo le due proprietà importanti del prodotto interno
$$
x\perp y\iff\langle x,y\rangle_T=0
$$
$$
||x||=\sqrt{\langle x,x\rangle_T}
$$
dove il quadrato del modulo è detta energia del segnale.

---
Ora che abbiamo definito come due segnali possano essere ortonormali, definiamo una [[Base ortonormale|base ortonormale]] come un insieme di funzioni $\{\psi_n\}$ definite sull'intervallo $T$, allora si avrà che un segnale $x$ è rappresentabile come [[Combinazione lineare|combinazione lineare]] di elementi della base
> [!remark] Combinazione lineare 
> $$
> x=x_1\psi_1+\dots+x_n\psi_n
> $$

e i coefficienti $x_k$ sono ottenibili con il prodotto interno con gli elementi della base
> [!remark] Estrazione dei coefficienti
> $$
> x_k=\langle x,\psi_k\rangle_T
> $$
---
Applicando questi concetti allo sviluppo di Fourier si ha che i termini della [[Forma esponenziale di segnali complessi|forma esponenziale]] sono ortogonali, ma non ortonormali
$$
\langle\phi_n,\phi_m\rangle_T=\int_Tdt\phi_n\phi_m^\dagger=\int_Tdt\e^{jn\omega_0t}\e^{-jn\omega_0t}=\int_Tdt\e^{j(m-n)\omega_0t}=\begin{cases}0&m\ne n\\ T&m=n\end{cases}
$$
allora con una semplice riscalamento si ottiene una base ortonormale
$$
\psi_n=\frac{1}{\sqrt{T}}\phi_n=\frac{1}{\sqrt{T}}\e^{jn\omega_0t}
$$
$$
\langle\psi_n,\psi_m\rangle_T=\begin{cases}0&m\ne n\\1&m=n\end{cases}
$$
allora un qualsiasi segnale è rappresentabile come
$$
x=\sqrt{T}\sum_{n=-\infty}^{+\infty}c_n\psi_n=\sqrt{T}\sum_{n=-\infty}^{+\infty}c_n\e^{jn\omega_0t}
$$