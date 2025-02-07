> [!definition] Trasformata di Steinmetz
> La trasformata di Steinmetz è una trasformata integrale di kernel $\frac{\sqrt{2}}{T}\e^{-j\omega t}$ che porta dal dominio del tempo al dominio dei [[Fasore|fasori]].
> $$
> \mathcal{S}[x]=\frac{\sqrt{2}}{T}\int_Tdtx\e^{-j\omega t}=\evec{X}
> $$
> `\begin{proof}`
> $$
> \mathcal{S}[x]=\frac{\sqrt{2}}{T}\int_Tdtx\e^{-j\omega t}=\frac{\sqrt{2}}{T}\int_Tdt\hat{X}\cos(\omega t+\varphi)\e^{-j\omega t}
> $$
> $$
> =\frac{\sqrt{2}\hat{X}}{T}\int_Tdt\frac{\e^{j(\omega t+\varphi)}+\e^{-j(\omega t+\varphi)}}{2}\e^{-j\omega t}=\frac{\hat{X}}{\sqrt{2}T}\left(\int_Tdt\e^{j\varphi}+\int_Tdt\e^{-j(2\omega t+\varphi)}\right)
> $$
> $$
> =\frac{\hat{X}}{\sqrt{2}T}\eval{t\e^{j\varphi}}{0}{T}=\frac{\hat{X}}{\sqrt{2}}e^{j\varphi}=X\e^{j\varphi}=\evec{X}
> $$
> `\end{proof}`

> [!remark] Linearità
> $$
> \mathcal{S}[\lambda x+\mu y]=\lambda\evec{X}+\mu\evec{Y}
> $$ 


> [!remark] Derivata
> $$
> \mathcal{S}[\dot{x}]=j\omega\mathcal{S}[x]
> $$
> `\begin{proof}`
> $$
> \mathcal{S}[\dot{x}]=\frac{\sqrt{2}}{T}\int_Tdt\frac{dx}{dt}\e^{-j\omega t}=\frac{\sqrt{2}}{T}\left(\eval{x\e^{-j\omega t}}{0}{T}+j\omega\int_Tdtx\e^{+j\omega t}\right)
> $$
> $$
> =j\omega\frac{\sqrt{2}}{T}\int_Tdtx\e^{-j\omega t}=j\omega\mathcal{S}[x]
> $$
> `\end{proof}`