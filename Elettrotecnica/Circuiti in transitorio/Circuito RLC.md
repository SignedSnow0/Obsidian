> [!definition] Diagramma
> ![lg](RLC.drawio.svg)

> [!definition] Circuito RLC
> Un circuito RLC è definito principalmente da 2 fattori
> * $\alpha=\frac{R}{2L}$ chiamato "fattore di smorzamento"
> * $\omega_0=\frac{1}{\sqrt{LC}}$ chiamato "pulsazione di risonanza"
>
> allora la soluzione si divide in 3 casi:
> * $\alpha>\omega_0$
> $$
> i=\frac{E-v_{C0}}{L\sqrt{\alpha^2-\omega_0^2}}\frac{\e^{\sqrt{\alpha^2-\omega_0^2}t}-\e^{-\sqrt{a^2-\omega_0^2}t}}{2}\e^{-\alpha t}
> $$
> * $\alpha=\omega_0$
> $$
> i=\frac{E-v_{C0}}{L}t\e^{-\alpha t}
> $$
> * $\alpha<\omega_0$
> $$
> i=\frac{E-v_{C_0}}{L\omega_d}\sin(\omega_dt)\e^{-\alpha t}
> $$
> dove $\omega_d^2=\omega_0^2-\alpha^2$
> 
> `\begin{proof}`
> Ad un istante $t_0$ l'interruttore si chiuderà, allora possiamo applicare l'[[Leggi di Kirchhoff|LKT]] per studiare il transitorio:
> $$
> E-v_R-v_L-v_C=0
> $$
> a questo punto indichiamo le leggi costitutive dei componenti:
> $$
> v_R=Ri
> $$
> $$
> v_L=L\frac{di}{dt}
> $$
> $$
> v_C=\frac{1}{C}\int dti
> $$
> allora applicandole all'equazione di prima si ha
> $$
> E-Ri-L\frac{di}{dt}-\frac{1}{C}\int dti=0
> $$
> derivando e riordinando si ha
> $$
> \frac{d^2i}{dt^2}+\frac{R}{L}\frac{di}{dt}-\frac{1}{LC}i=0
> $$
> il [[Polinomio caratteristico di un ODE lineare a coefficienti costanti|polinomio caratteristico]] dell'[[ODE lineare]] è
> $$
> \lambda^2+\frac{R}{L}\lambda+\frac{1}{LC}=0
> $$
> e i suoi zeri sono:
> $$
> \lambda_{1,2}=\frac{R}{2L}\pm\sqrt{\left(\frac{R}{2L}\right)^2-\frac{1}{LC}}=-\alpha\pm\sqrt{\alpha^2-\omega_0^2}
> $$
> a questo punto dividiamo il procedimento in 3 casi:
> * $\alpha>\omega_0$
> dato che abbiamo due zeri reali e distinti la soluzione generale sarà della forma
> $$
> i=A_1\e^{\lambda_1t}+A_2\e^{\lambda_2t}
> $$
> applichiamo ora le condizioni iniziali
> $$
> \evals{i}{t=t_0}=0=A_1+A_2\implies A_1=-A_2
> $$
> $$
> \evals{v}{t=t_0}=\left[E-Ri-L\frac{di}{dt}-v_C\right]_{t=t_0}=E-L\frac{di}{dt}-v_{C_0}=0\implies
> $$
> $$
> \evals{\frac{di}{dt}}{t=t_0}=\frac{E-v_{C_0}}{L}=A_1\lambda_1-A_2\lambda_2=2A_1\sqrt{\alpha^2-\omega_0^2}
> $$
> $$
> \implies A_1=-A_2=\frac{E-v_{C_0}}{2L\sqrt{\alpha^2-\omega_0^2}}
> $$
> allora la soluzione diventa
> $$
> i=\frac{E-v_{C_0}}{L\sqrt{\alpha^2-\omega_0^2}}\frac{\e^{\sqrt{\alpha^2-\omega_0^2}t}-\e^{-\sqrt{\alpha^2-\omega_0^2}t}}{2}\e^{-\alpha t}
> $$
> * $\alpha=\omega_0$
> allora avremo uno zero reale con [[Molteplicità algebrica|m.a]] pari a due, la soluzione generale è della forma
> $$
> i=A_1\e^{-\alpha t}+A_2t\e^{-\alpha t}
> $$ 
> applichiamo ancora le condizioni iniziali
> $$
> \evals{i}{t=t_0}=0=A_1
> $$
> $$
> \evals{\frac{di}{dt}}{t=t_0}=\frac{E-v_{C_0}}{L}=A_2
> $$
> allora la soluzione diventa
> $$
> i=\frac{E-v_{C_0}}{L}t\e^{-\alpha t}
> $$
> * $\alpha<\omega_0$
> allora avremo due zeri complessi e coniugati, definiamo
> $$
> \omega_d=\omega_0^2-\alpha^2
> $$
> sostituendo alla soluzione del primo caso si ha
> $$
> i=\frac{E-v_{C_0}}{Lj\omega_d}\frac{\e^{j\omega_dt}-\e^{-j\omega_dt}}{2}\e^{-\alpha t}=\frac{E-v_{C_0}}{Lj\omega_d}\cos(\omega_dt)\e^{-\alpha t}
> $$
> $$
> =\frac{E-v_{C_0}}{L\omega_d}\sin(\omega_dt)\e^{-\alpha t}
> $$
> `\end{proof}`