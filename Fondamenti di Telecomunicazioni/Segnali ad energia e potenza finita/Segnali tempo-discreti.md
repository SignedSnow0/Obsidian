Per i segnali tempo discreti le definizioni precedenti sono portate dal caso continuo al discreto
> [!definition] Energia
> $$
> E=\sum_{n=-\infty}^{+\infty}|x_n|^2
> $$

> [!definition] Potenza
> $$
> P=\langle|x_n|^2\rangle=\lim_{N\to\infty}\frac{1}{2N+1}\sum_{n=-N}^{+N}|x_n|^2
> $$

> [!definition] Autocorrelazione
> Per energia finita
> $$
> \dot{c_k}=\sum_{n=-\infty}^{+\infty}x_n^\dagger x_{n+k}
> $$
> per potenza finita
> $$
> c_k=\langle x_n^\dagger,x_{n+k}\rangle=\lim_{N\to\infty}\frac{1}{2N+1}\sum_{n=-N}^{+N}x_n^\dagger x_{n+k}
> $$