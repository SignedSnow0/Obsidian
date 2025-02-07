> [!definition] Diagramma
>![lg](RL.drawio.svg)

> [!definition] Circuito RL
> Il voltaggio in un circuito RL è definito da 
> $$
> i=\left(v_0-\frac{E}{R}\right)\e^{-\frac{R}{L}t}+\frac{E}{R}
> $$
> `\begin{proof}`
> Ad un certo istante l'interruttore si chiuderà, sarà allora possibile applicare l'[[Leggi di Kirchhoff|LKT]] alla maglia:
> $$
> E-v_R-v_L=0
> $$
> applichiamo le equazioni costitutive
> $$
> v=Ri
> $$
> $$
> v=\frac{di}{dt}
> $$
> si ha allora
> $$
> E-Ri-L\frac{di}{dt}=0
> $$
> $$
> \frac{di}{dt}+\frac{R}{L}i=\frac{E}{L}
> $$
> risolviamo l'[[ODE lineare]]: risolviamo l'[[ODE lineare omogenea associata|omogenea associata]] con il [[Polinomio caratteristico|polinomio caratteristico]]
> $$
> P(\lambda)=\lambda+\frac{R}{L}
> $$
> $$
> \lambda_1=-\frac{R}{L}
> $$
> otteniamo quindi il seguente [[Sistema fondamentale di soluzioni|sistema fondamentale di soluzioni]]
> $$
> A_1\e^{-\frac{R}{L}t}
> $$
> riguardo la soluzione particolare sappiamo che ha andamento pari al termine costante $\frac{E}{R}$, allora
> $$
> i=\frac{E}{R}
> $$
> allora la soluzione sarà
> $$
> A_1\e^{-\frac{R}{L}t}+\frac{E}{R}
> $$
> dato che al tempo $t_0=0$ la tensione sarà $v_0$ si ha
> $$
> \left[A_1\e^{-\frac{R}{L}}+\frac{E}{R}\right]_{t=0}=A_1+\frac{E}{R}=v_0\implies A_1=v_0-\frac{E}{R}
> $$
> allora la soluzione generale è
> $$
> i=\left(v_0-\frac{E}{R}\right)\e^{-\frac{R}{L}t}+\frac{E}{R}
> $$
> `\end{proof}`