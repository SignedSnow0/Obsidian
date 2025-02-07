> [!theorem] Teorema di Noether
> Ogni simmetria continua della densità lagrangiana $\mathcal{L}$ porta ad una corrente di Noether $\mathcal{J}^\mu$ tale che 
> $$
> \partial_\mu\mathcal{J}^\mu=0
> $$
> che rappresenta una quantità conservata.
> `\begin{proof}`
> Definiamo una trasformazione del campo $\phi$
> $$
> \phi'=\phi+\epsilon\delta\phi+o\left(\epsilon^2\right)
> $$
> ricordiamo che la variazione dipende dal campo che dalla sua derivata:
> $$
> \delta\phi=X(\phi,\partial_\mu\phi)
> $$
> Analizziamo ora la variazione della lagrangiana:
> $$
> \mathcal{L}'=\mathcal{L}+\epsilon\delta\mathcal{L}+o\left(\epsilon^2\right)
> $$
> allora
> $$
> \delta\mathcal{L}=\partial_\mu F^\mu=\frac{\partial\mathcal{L}}{\partial\phi}\delta\phi+\frac{\partial\mathcal{L}}{\partial(\partial_\mu\phi)}\delta(\partial_\mu\phi)
> $$
> dalla derivata del prodotto si ha
> $$
> \partial_\mu\left(\frac{\partial\mathcal{L}}{\partial(\partial_\mu\phi)}\delta\phi\right)=\partial_\mu\frac{\partial\mathcal{L}}{\partial(\partial_\mu\phi)}\delta\phi+ \frac{\partial\mathcal{L}}{\partial(\partial_\mu\phi)}\delta(\partial_\mu\phi)
> $$
> si ha
> $$
> \delta\mathcal{L}=\partial_\mu F^\mu=\frac{\partial\mathcal{L}}{\partial\phi}\delta\phi+\partial_\mu\left(\frac{\partial\mathcal{L}}{\partial(\partial_\mu\phi)\delta\phi}\right)-\delta_\mu\frac{\partial\mathcal{L}}{\partial(\partial_\mu\phi)}\delta\phi
> $$
> raccogliendo
> $$
> \partial_\mu\left(\frac{\partial\mathcal{L}}{\partial(\partial_\mu\phi)}\delta\phi-F^\mu\right)=-\left(\frac{\partial\mathcal{L}}{\partial\phi}-\partial_\mu\frac{\delta\mathcal{L}}{\partial(\partial_\mu\phi)}\right)\delta\phi
> $$
> notando che la parentesi a destra sono le equazioni di eulero-lagrange e per ipotess esse sono costanti nella trasformazione si ha che la parte sinistra è nulla:
> $$
> \mathcal{J}^\mu=\frac{\partial\mathcal{L}}{\partial(\partial_\mu\phi)}\delta\phi-F^\mu\implies\delta_\mu\mathcal{J}^\mu=0
> $$
> `\end{proof}`