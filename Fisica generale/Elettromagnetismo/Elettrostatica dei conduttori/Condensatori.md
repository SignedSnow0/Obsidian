---
subject: fisica generale
type: definizione
---
Un condensatore è un sistema di due conduttori carichi dove si verifica [[Induzione completa]].
I due conduttori si chiamano armature e lo spazio fra le armature si chiama intercapedine.
La capacità di un condensatore è definito come il rapporto della carica sulla differenza di potenziale delle due armature
$$
C=\frac{Q}{\Delta V}
$$
Per un condensatore piano la capacità vale
$$
C=\frac{\epsilon_0S}{d}
$$
per un condensatore sferico
$$
C=4\pi\epsilon_0\left(\frac{R_1R_2}{R_2-R_1}\right)
$$
---
L'energia elettrostatica accumulata è 

$$
d\mathcal{L}=dq\Delta V_q=dq\frac{q}{C}
$$
$$
L=\int_0^Qd\mathcal{L}=\int_0^Qdq\frac{q}{C}=\frac12\frac{Q^2}{C}=\frac12Q\Delta V
$$
Riscrivendo la formula otteniamo
$$
U_e=\frac12Q\Delta V=\frac12C\Delta V^2=\frac12\frac{\epsilon_0S}{d}(Ed)^2=\frac12\epsilon_0dSE^2=(\frac12\epsilon_0E^2)(dS)
$$
allora definendo $\frac12\epsilon_0E^2$ come densità di energia $u_e$ elettrostatica si ha che l'energia in un condensatore è la densità di energia per il volume ($dS$)
$$
U_e=\iiint_Vu_edV
$$
---
Per sistemi di condensatori si ha
* Se i condensatori sono disposti in serie (un polo in comune) la capacità equivalente è

* Se i condensatori sono disposti in parallelo (stessa differenza di potenziale) la capacità equivalente è
$$
C_{\text{eq}}=\sum C_i
$$