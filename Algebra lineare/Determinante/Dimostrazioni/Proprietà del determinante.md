---
subject: algebra lineare
type: dimostrazione
---
1. Se $A$ ha due righe uguali o una riga nulla, allora $\det A=0$
2. Il [[Determinante|determinante]] è [[Applicazione lineare|lineare]] rispetto alla somma delle righe

$$
A=\begin{pmatrix}a_{11}&\dots&a_{1n}\\\vdots&\vdots&\vdots\\b_{i1}+c_{1i1}&\dots&b_{in}+c_{in}\\\vdots&\vdots&\vdots\\a_{n1}&\dots&a_{nn}\end{pmatrix}\quad A_1=\begin{pmatrix}a_{11}&\dots&a_{1n}\\\vdots&\vdots&\vdots\\b_{i1}&\dots&b_{in}\\\vdots&\vdots&\vdots\\a_{n1}&\dots&a_{nn}\end{pmatrix}\quad A_2=\begin{pmatrix}a_{11}&\dots&a_{1n}\\\vdots&\vdots&\vdots\\c_{1i1}&\dots&c_{in}\\\vdots&\vdots&\vdots\\a_{n1}&\dots&a_{nn}\end{pmatrix}
$$
$$
\det A=\det A_1+\det A_2
$$
3. Il [[Determinante|determinante]] è [[Applicazione lineare|lineare]] rispetto al prodotto di una riga con uno scalare

$$
\det\begin{pmatrix}a_{11}&\dots&a_{1n}\\\vdots&\ddots&\vdots\\\lambda a_{i1}&\dots&\lambda a_{in}\\\vdots&\ddots&\vdots\\a_{nn}&\dots&a_{nn}\end{pmatrix}=\lambda\det\begin{pmatrix}a_{11}&\dots&a_{1n}\\\vdots&\ddots&\vdots\\a_{i1}&\dots& a_{in}\\\vdots&\ddots&\vdots\\a_{nn}&\dots&a_{nn}\end{pmatrix}
$$
4. Se $A'$ è la matrice ottenuta scambiando due righe di $A$, allora $\det A=-\det A'$
5. Per ogni [[Matrice triangolare|matrice triangolare superiore]] $\det A=a_{11}\dots a_{nn}$
6. $\det A=\det^tA$
7. Teorema di Binet $\forall A,B\in\mathbb{R}^{n,n}\quad det(AB)=\det A\det B$