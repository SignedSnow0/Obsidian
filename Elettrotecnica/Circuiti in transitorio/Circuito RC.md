> [!definition] Circuito RC
> ![lg](RC.drawio.svg)
> ---
> La corrente in un circuito RC è definita da
> $$
> i=(v_0-E)\e^{-\frac{t}{RC}}+E
> $$
> * La costante $\frac{1}{RC}$ è chiamata
> 
> `\begin{proof}`
> Al tempo $t_0=0$ l'interruttore si chiude, possiamo quindi applicare l'[[Leggi di Kirchhoff|LKT]] ottenendo
> $$
> E-v_R-v_C=0
> $$
> dalle equazioni costitutive sappiamo che
> $$
> v_R=Ri
> $$
> $$
> i=C\frac{dv_C}{dt}
> $$
> dato che le due correnti sono equivalenti possiamo unire le equazioni
> $$
> v_R=RC\frac{dv_C}{dt}
> $$
> tornando alla legge delle maglie si ha
> $$
> E-RC\frac{dv_C}{dt}-v_C=0
> $$
> $$
> \frac{dv_C}{dt}+\frac{v_C}{RC}=\frac{E}{RC}
> $$
> usiamo il [[Metodo di variazione delle costanti|il metodo di variazione delle costanti]] per risolvere l'[[ODE lineare]]: troviamo la soluzione all'[[ODE lineare omogenea associata|omogenea associata]]
> $$
> P(\lambda)=\lambda+\frac{1}{RC}
> $$
> $$
> \lambda_1=-\frac{1}{RC}
> $$
> il [[Sistema fondamentale di soluzioni|sistema fondamentale di soluzioni]] è quindi
> $$
> A_1\e^{-\frac{t}{RC}}
> $$
> riguardo la soluzione particolare sappiamo che l'andamento è pari alla costante $\frac{E}{RC}$, allora
> $$
> \frac{v_C}{RC}=\frac{E}{RC}\implies v_c=E
> $$
> allora la soluzione generale è
> $$
> A_1\e^{-\frac{t}{RC}}+E
> $$
> dato che per $t=0$ il voltaggio iniziale è $v_0$ si ha 
> $$
> \left[A_1\e^{-\frac{t}{RC}}+E\right]_{t=0}=A_1+E=v_0
> $$
> $$
> A_1=v_0-E
> $$
> allora la soluzione al circuito è
> $$
> i=(v_0-E)\e^{-\frac{t}{RC}}+E
> $$
> `\end{proof}`