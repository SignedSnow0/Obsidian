---
subject: fisica generale
type: definizione
---
In un [[Sistema isolato|sistema]] di [[Punto materiale|punti materiali]] è utile studiare una classe di forze che agiscono fra più punti per un periodo di tempo molto breve: gli urti.
* Nello studio degli urti si è interessati non alla maniera in cui interagiscono i [[Punto materiale|corpi]], ma solamente al risultato finale, cioè le differenze nei moti dei corpi interessati, un urto perciò è strettamente collegato al concetto di [[Impulso|impulso]], dove un [[Impulso|impulso]] di tempo ristretto è considerato un urto.
* Se i due corpi non sono vincolati, le uniche forze che agiscono sono quelle [[Sistema isolato|interne al sistema]], perciò i punti avranno solamente una differenza di [[Inerzia|inerzia]]
$$
\int_{t_1}^{t_2}\vec{F}dt=\vec{q}(t_2)-\vec{q}(t_1)
$$
* A parità di forza si avrà che l'intensità dell'urto è maggiore per intervalli di tempo più piccoli
$$
\langle\vec{F}\rangle=\avint_{t_1}^{t_2}\vec{F}dt=\frac{\vec{q}(t_2)-\vec{q}(t_1)}{\Delta t}
$$
---
Se gli urti sono perfettamente elastici allora l'[[Energia cinetica|energia cinetica]] è conservata, perciò abbiamo il sistema
$$
\begin{cases}Q_i=Q_o\\K_i=K_o\end{cases}=\begin{cases}m_1v_{1,i}+m_2v_{2,i}=m_1v_{1,o}+m_2v_{2,o}\\\displaystyle\frac12m_1v_{1,i}^2+\frac12m_2v_{2,i}^2=\frac12m_1v_{1,o}^2+\frac12m_2v_{2,o}^2\end{cases}
$$
allora
$$
v_{1,o}=\frac{m_1-m_2}{m_1+m_2}v_{1,i}+\frac{2m_2}{m_1+m_2}v_{2,i}
$$
$$
v_{2,o}=\frac{2m_1}{m_1+m_2}v_{1,i}+\frac{m_2-m_1}{m_1+m_2}v_{2,i}
$$
in particolare se le due masse sono uguali $m_1=m_2$
$$
v_{1,o}=v_{2,i}\quad v_{2,o}=v_{1,i}
$$
se una massa è molto diversa $m_1>>m_2$
$$
v_{1,o}=v_{1,i}\quad v_{2,o}=2v_{1,i}-v_{2,i}
$$
---
Se invece l'urto sarà totalmente plastico si avrà che le due masse rimarranno attaccate quindi con la stessa velocità $v_{1,o}=v_{2,o}=v_o$
$$
m_1v_{1,i}=m_2v_{2,i}=(m_1+m_2)v_o
$$