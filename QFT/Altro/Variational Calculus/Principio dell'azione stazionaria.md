Definiamo l'azione come
$$
\mathcal{S}=\int_{t_1}^{t_2}(K-U)dt
$$
allora il percorso che un [[Punto materiale|punto materiale]] sceglie è quello dove l'azione è un [[Punto critico|punto stazionario]].
1. Definiamo allora il minimo di $\mathcal{S}$: P
Prendiamo una funzione generica $f(x)$, facciamo il suo [[Sviluppo di Taylor con resto di Peano|sviluppo di Taylor]]
$$
f(x+\epsilon)=f(x)+\epsilon\frac{df}{dx}+\epsilon^2\frac{d^2f}{dx^2}+\dots
$$
$$
\Delta f=f(x+\epsilon)-f(x)=\epsilon\frac{df}{dx}+\epsilon^2\frac{d^2f}{dx^2}+\dots
$$
ma se $x$ è [[Punto critico|punto critico]] per $f$ allora $\frac{df}{dx}=0$, quindi
$$
\Delta f=\epsilon^2\frac{d^2f}{dx^2}+\dots
$$
abbiamo ottenuto quindi che per un [[Punto critico|punto critico]] di $f$ il primo cambiamento della funzione è almeno al secondo ordine.
2. Torniamo ora all'azione: in questo caso invece di dover trovare un punto $x$ in cui $\mathcal{S}$ è critico, dobbiamo trovare una funzione che rappresenta il percorso di $\mathcal{S}$ in cui l'azione è minima su tutto di esso.
3. Definiamo il percorso che cerchiamo come $x(t)$, e un deviazione da $x$ con un altra funzione $\eta(t)$, allora per l'azione
$$
\mathcal{S}=\int_{t_1}^{t_2}\left[\frac12m\left(\frac{dx}{dt}\right)^2-U(x)\right]dt
$$
la differenza tra il vero percorso $x(t)$ e la deviazione $x(t)+\eta(t)$ dovrebbe avere una variazione $\delta\mathcal{S}$ uguale a $0$ al primo ordine per il punto $1$
$$
\delta\mathcal{S}=\mathcal{S}(x+\eta)-S(x)=0
$$
4. Analizziamo ora $\mathcal{S}(x+\eta)$
$$
\mathcal{S+\eta}=\int_{t_1}^{t_2}\left[\frac12m\left(\frac{d}{dt}(x+\eta)\right)^2-U(x+\eta)\right]dt=
$$
$$
=\int_{t_1}^{t_2}\left[\frac12m\left(\frac{dx}{dt}+\frac{d\eta}{dt}\right)^2-U(x+\eta)\right]dt
$$
$$
\left(\frac{dx}{dt}+\frac{d\eta}{dt}\right)^2=\left(\frac{dx}{dt}\right)^2+\left(\frac{d\eta}{dt}\right)^2+2\frac{dx}{dt}\frac{d\eta}{dt}
$$
visto che siamo interessati al cambiamento al primo ordine dell'azione possiamo ignorare $\eta$ al secondo ordine:
$$
\left(\frac{dx}{dt}+\frac{d\eta}{dt}\right)^2=\left(\frac{dx}{dt}\right)^2+2\frac{dx}{dt}\frac{d\eta}{dt}
$$
espandiamo con [[Sviluppo di Taylor con resto di Peano|Taylor]] il [[Potenziale|potenziale]]:
$$
U(x+\eta)=U(x)+\eta\frac{dU}{dx}+\frac{\eta^2}{2!}\frac{d^2U}{dx^2}+\dots
$$
e come prima ignoriamo gli ordini successivi al primo, allora con po di riordinamento si ha
$$
\mathcal{S}(x+\eta)=\int_{t_1}^{t_2}\left[\frac12m\left(\frac{dx}{dt}\right)^2-U(x)+\frac12m\left(2\frac{dx}{dt}\frac{d\eta}{dt}\right)-\eta\frac{dU}{dx}\right]dt
$$
5. Ricordiamo ciò che vogliamo ottenere: $\delta\mathcal{S}=\mathcal{S}(x+\eta)-\mathcal{S}(x)=0$
$$
\delta\mathcal{S}=\int_{t_1}^{t_2}\left[\frac12m\left(\frac{dx}{dt}\frac{d\eta}{dt}\right)-\eta\frac{dU}{dx}\right]dt=0
$$
Integriamo ora $\frac{dx}{dt}\frac{d\eta}{dt}$ per parti:
$$
\int_{t_1}^{t_2}\frac{dx}{dt}\frac{d\eta}{dt}dt=\eval{\frac{dx}{dt}\eta}{t_1}{t_2}-\int_{t_1}^{t^2}\frac{d^2x}{dt^2}\eta dt
$$
ricordiamo ora che $\eta$ rappresenta la deviazione dal percorso originale, che però sara $0$ agli estremi del percorso perchè ogni cammino avrà per ipotesi stessa partenza e stessa destinazione, perciò
$$
\eval{\frac{dx}{dt}\eta}{t_1}{t_2}=0
$$
allora 
$$
\delta{S}=\int_{t_1}^{t_2}\left[-\frac12m\frac{d^2x}{dt^2}\eta-\frac{dU}{dt}\eta\right]dt=\int_{t_1}^{t_2}\left[-\frac12m\frac{d^2x}{dt^2}-\frac{dU}{dt}\right]\eta dt=0
$$
ottenendo ora una formula dove il prodotto di due fattori sono uguali a $0$, perciò
$$
-\frac12m\frac{d^2x}{dt^2}-\frac{dU}{dt}=0\implies\frac12m\frac{d^2x}{dt^2}=-\frac{dU}{dt}
$$
che è
$$
F=ma
$$
per un [[Moto rettilineo uniforme|moto rettilineo]]
Abbiamo quindi trovato che il percorso che minimizza l'azione usata è quello seguito dal [[Secondo principio della dinamica|secondo principio della dinamica]].