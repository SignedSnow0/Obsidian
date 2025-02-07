---
subject: fondamenti di telecomunicazioni
---
Poiché i coefficienti di un segnale sono complessi, essi vengono rappresentati con due grafici che ne rappresentano l'ampiezza ($A_n=|c_n|$) e la fase ($\phi_n=\angle c_n$), e dato che i coefficienti sono quantità discrete sono disposti in un grafico a pettine in punti equidistanti a multipli di $\omega_0$.
#### Diagramma dell'ampiezza
```tikz 
\begin{document} 
\begin{tikzpicture}[domain=-4:5] 
	\draw[->] (-4,0) -- (5,0) node[right] {$\omega$};
	\draw[->] (-4,0) -- (-4,4) node[right] {$|c_n|$};
	\draw (-3,2) -- (-3,0) node[below] {$-3\omega_0$};
	\draw (-2,1) -- (-2,0) node[below] {$-2\omega_0$};
	\draw (-1,3) -- (-1,0) node[below] {$-\omega_0$};
	\draw (0,2) -- (0,0) node[below] {$0$};
	\draw (1,1) -- (1,0) node[below] {$\omega_0$};
	\draw (2,2) -- (2,0) node[below] {$2\omega_0$};
	\draw (3,1) -- (3,0) node[below] {$3\omega_0$};
	
	\draw[fill] (-3,2) circle [radius=0.1cm];
	\draw[fill] (-2,1) circle [radius=0.1cm];
	\draw[fill] (-1,3) circle [radius=0.1cm];
	\draw[fill] (0,2) circle [radius=0.1cm];
	\draw[fill] (1,1) circle [radius=0.1cm];
	\draw[fill] (2,2) circle [radius=0.1cm];
	\draw[fill] (3,1) circle [radius=0.1cm];
\end{tikzpicture}
\end{document} 
```
#### Diagramma dell'argomento
```tikz 
\begin{document} 
\begin{tikzpicture}[domain=-4:5] 
	\draw[->] (-4,0) -- (5,0) node[right] {$\omega$};
	\draw[->] (-4,0) -- (-4,4) node[right] {$\angle c_n$};
	\draw[-.] (-3,-1) -- (-3,0) node[midway,right] {$-3\omega_0$};
	\draw (-2,1) -- (-2,0) node[midway,right] {$-2\omega_0$};
	\draw (-1,-2) -- (-1,0) node[midway,right] {$-\omega_0$};
	\draw (0,2) -- (0,0) node[midway,right] {$0$};
	\draw (1,1) -- (1,0) node[midway,right] {$\omega_0$};
	\draw (2,-2) -- (2,0) node[midway,right] {$2\omega_0$};
	\draw (3,2) -- (3,0) node[midway,right] {$3\omega_0$};

	\draw[fill] (-3,-1) circle [radius=0.1cm];
	\draw[fill] (-2,1) circle [radius=0.1cm];
	\draw[fill] (-1,-2) circle [radius=0.1cm];
	\draw[fill] (0,2) circle [radius=0.1cm];
	\draw[fill] (1,1) circle [radius=0.1cm];
	\draw[fill] (2,-2) circle [radius=0.1cm];
	\draw[fill] (3,2) circle [radius=0.1cm];
\end{tikzpicture}
\end{document} 
```
Dato che le pulsazioni possono essere sia positive che negative, lo spettro si dice bilatero, dove una pulsazione positiva corrisponde ad una rotazione antioraria del fasore, e una rotazione oraria corrisponde ad una pulsazione negativa.