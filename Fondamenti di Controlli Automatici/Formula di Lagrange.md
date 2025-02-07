> [!theorem] Formula di Lagrange
> Dato un [[Sistema dinamico tempo continuo|sistema lineare]] con stato iniziale $\vec{x}(t_0)=\vec{x}_{t_0}$, la soluzione del movimento dello stato è
> $$
> \vec{x}=\e^{\mathbf{A}(t-t_0)}\vec{x}_{t_0}+\int_{t_0}^{t}d\tau\e^{\mathbf{A}(t-\tau)}\mathbf{B}\vec{u}(t-\tau)
> $$
> e il movimento di uscita risulterà
> $$
> \vec{y}=\mathbf{C}\e^{\mathbf{A}(t-t_0)}\vec{x}_{t_0}+\mathbf{C}\int_{t_0}^{t}d\tau\e^{\mathbf{A}(t-\tau)}\mathbf{B}\vec{u}(\tau)+\mathbf{D}\vec{u}
> $$

