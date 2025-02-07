---
subject: fondamenti di telecomunicazioni
---
Nella teoria della modulazione esistono due segnali principali
* Il segnale da trasmettere $x$, in generale passa basso, reale e di valor medio nullo, chiamato segnale modulante.
* Il segnale che trasmette $x$ chiamato portante $s$, passa banda, ottenuto dalla modulazione di $x$

> [!definition] Portante
> La portante è un segnale sinusoidale caratterizzato da valori pre modulazione
> $$
> s_0=V_0\cos(\omega_0t-\phi_0)
> $$

> [!definition] Portante modulata
> Il segnale portante viene alterato in fase o ampiezza in modo da portare nelle variazione dai valori base le informazioni del segnale modulante, la sua equazione risulta:
> $$
> s=V\cos\phi
> $$
> * $V$ è detta ampiezza istantanea.
> * $\phi$ è detta fase istantanea.
> * $\omega=\dot\phi$ è detta pulsazione istantanea.

> [!definition] Deviazioni
> Esistono altri parametri chiamati deviazioni che indicano la differenza fra i valori della portante base e quella modulata:
> * $V-V_0$ deviazione istantanea di ampiezza.
> * $m=\frac{V-V_0}{V_0}$ deviazione istantanea relativa di ampiezza.
> * $\alpha=\phi-(\omega_0t-\phi_0)$ deviazione istantanea di fase.
> * $\Delta\omega=\omega-\omega_0$ deviazione istantanea di pulsazione.
>
> La deviazione di fase e pulsazione sono legate tramite la formula
> $$
> \Delta\omega=\dot\alpha
> $$
> $$
> \alpha=\int_{-\infty}^{t}d\tau\Delta\omega
> $$
> allora la portante modulata è esprimibile in termine delle sue deviazioni:
> $$
> s=V_0(1+m)\cos(\alpha+\omega_0t-\phi_0)
> $$