Dall'[[Autoinduzione|autoinduzione]] abbiamo visto che un'induttanza si comporta come un generatore di [[Forza elettromotrice|forza elettromotrice]] opposta alla variazione di corrente.
$$
\mathcal{E}_{\text{ind}}=-L\frac{di}{dt}
$$
possiamo quindi ricavare l'espressione del lavoro necessario per contrastare la forza indotta con la definizione di [[Intensità di corrente|corrente]] e la formula ricavata prima:
$$
\delta\mathcal{L}=-\mathcal{E}_{\text{ind}}dq=-\left(-L\frac{di}{dt}\right)(idt)
$$
allora il lavoro compiuto per portare il circuito da una corrente $i_0=0$ a $i$ è
$$
\mathcal{L}=\int_0^iLidi=\frac12Li^2
$$
perciò l'energia magnetica accumulata da un [[Autoinduzione|induttanza]] è 
$$
U_B=\frac12Li^2
$$
Inoltre ricordando l'espressione di induttanza di un solenoide
$$
L=\mu_0\frac{N^2}{l}S
$$
il campo magnetico invece vale
$$
B=\mu_0\frac{N}{l}i\implies i=\frac{Bl}{\mu_0 N}
$$
allora 
$$
U_B=\frac12Li^2=\frac12\left(\mu_0\frac{N^2}{l}S\right)\left(\frac{Bl}{\mu_0N}\right)^2=\frac{B^2}{2\mu_0}(lS)
$$
allora ponendo la densità di energia magnetica
$$
u_B=\frac{B^2}{2\mu_0}
$$
si ha per una qualsiasi volume
$$
U_B=\iiint_V u_BdV
$$