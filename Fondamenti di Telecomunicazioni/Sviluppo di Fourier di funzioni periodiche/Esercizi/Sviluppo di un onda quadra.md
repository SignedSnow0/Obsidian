---
subject: fondamenti di telecomunicazioni
---
Calcolare lo sviluppo di un onda quadra di ampiezza $A$, durata $\tau$ e periodo $T$.
Dato che lo [[Forma esponenziale di segnali complessi|sviluppo]] è [[Proprietà dello sviluppo di Fourier|tempo invariante]] centriamo un impulso nell'origine e calcoliamone i coefficienti $c_n$
$$
c_n=\frac{1}{T}\int_Tdtx\e^{-jn\omega_0 t}=\frac{1}{T}\int_{-\frac{\tau}{2}}^{\frac{\tau}{2}}dtA\e^{-jn\omega_0 t}=\frac{A}{T}\left[\frac{\e^{-jn\omega_0 t}}{-jn\omega_0}\right]_{-\frac{\tau}{2}}^{\frac{\tau}{2}}
$$
$$
=\frac{A}{T}\frac{\e^{-jn\omega_0\frac{\tau}{2}}-\e^{jn\omega_0\frac{\tau}{2}}}{jn\omega_0}=\frac{A}{T}\frac{-2\sin(n\omega_0\frac{\tau}{2})}{-jn\omega_0}
$$
$$
=\frac{A\tau}{T}\frac{\sin(n\omega_0\frac{\tau}{2})}{n\omega_0\frac{\tau}{2}}=\frac{I}{T}\sinc\left(n\frac{\tau}{T}\right)
$$
Allora ricaviamo i valori degli [[Spettri di ampiezza e fase bilateri|spettri di ampiezza e fase]]
$$
A_0=c_0=\frac{I}{T}
$$
$$
A_n=|2c_n|\frac{2I}{T}\left|\sinc\left(n\frac{\tau}{T}\right)\right|
$$
$$
\phi_n=-\angle c_n=\begin{cases}0&c_n>0\\\pi&c_n<0\end{cases}
$$