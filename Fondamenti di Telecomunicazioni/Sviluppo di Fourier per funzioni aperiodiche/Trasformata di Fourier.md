---
subject: fondamenti di telecomunicazioni
---
La trasformata di Fourier va a generalizzare i concetti della [[Forma esponenziale di segnali complessi|serie di Fourier]] per segnali aperiodici
> [!definition] Trasformata di Fourier
> $$
> X(\omega)=\int_{-\infty}^{+\infty}dtx(t)\e^{-j\omega t}
> $$

> [!definition] Antitrasformata di Fourier
> $$
> x(t)=\frac{1}{2\pi}\int_{-\infty}^{+\infty}d\omega X(\omega)\e^{j\omega t}
> $$


analogamente alla serie di Fourier, i termini $X(\omega)e^{j\omega t}d\omega$ rappresentano infinitesimi coefficienti della [[Forma esponenziale di segnali complessi|rappresentazione esponenziale]] di ampiezza $|X|$ e fase $\angle X$. 
Allora il [[Spettri di ampiezza e fase bilateri|diagramma degli spettri]] diventa il diagramma di una funzione continua dell'ampiezza
```tikz 
\begin{document} 
\begin{tikzpicture}[domain=-5:5] 
	\draw[->] (-5,0) -- (5,0) node[right] {$\omega$};
	\draw[->] (0,-2) -- (0,5) node[right] {$|X|$};
	\draw[thick] (-4,0) -- (-1,3) node[at start, below] {$-\omega_m$};
	\draw[thick] (1, 3) -- (4, 0) node[at end, below] {$\omega_m$};
	\draw[dashed] (-1, 0) -- (-1, 3) node[at start, below] {$-\omega_k$};
	\draw[dashed] (1, 0) -- (1, 3) node[at start,below] {$\omega_k$};

\end{tikzpicture}
\end{document} 
```
e della fase
```tikz 
\begin{document} 
\begin{tikzpicture}[domain=-5:5] 
	\draw[->] (-5,0) -- (5,0) node[right] {$\omega$};
	\draw[->] (0,-4) -- (0,4) node[right] {$\angle X$};
	\draw[thick] (-1,1) .. controls (-3.5,1.4) .. (-4,3);
	\draw[thick] (1,-1) .. controls (3.5,-1.4) .. (4,-3);
	\draw[dashed] (-4, 0) -- (-4, 3) node[at start, below] {$-\omega_m$};
	\draw[dashed] (-1, 0) -- (-1, 1) node[at start, below] {$-\omega_k$};
	\draw[dashed] (1, 0) -- (1, -1) node[at start,above] {$\omega_k$};
	\draw[dashed] (4, 0) -- (4, -3) node[at start,above] {$\omega_m$};

\end{tikzpicture}
\end{document} 
```