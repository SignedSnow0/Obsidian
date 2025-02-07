---
subject: fondamenti di telecomunicazioni
---
> [!definition] AM
> $$
> \text{AM}=\begin{cases}m=kx\\\alpha=0\end{cases}
> $$
> allora la [[Introduzione|portante modulata]] risulterà
> $$
> s=V_0(1+kx)\cos(\omega_0t-\phi_0)
> $$

> [!definition] Indice di modulazione AM
> L'indice di modulazione AM è definito come
> $$
> m_a=\max\{|m|\}\quad m_a\in[0,1]
> $$
> Il valore indica il livello di modulazione dove 0 indica assenza totale e 1 indica modulazione massima.
> Il valore è limitato fra $[0,1]$ perché $m\ge-1$ per definizione, $V\ge0$ e il segnale modulante ha valore medio nullo, quindi $m\in[-1,1]$. 

> [!definition] Sovramodulazione AM
> Se il segnale va in sovramodulazione, cioè
> $$
> m_a=kM>1\implies M>\frac{1}{k}
> $$
> la modulazione diventa ibrida
> $$
> \text{AM}=\begin{cases}V=V_0|1+kx|\\\alpha=\begin{cases}0&1+kx>0\\\pi&1+kx<0\end{cases}\end{cases}
> $$
> 