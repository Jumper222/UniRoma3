---
tags:
  - Probabilità_e_statistica
---
Il Metodo dei Momenti per la [[Stima Parametrica]] si tratta di studiare i momenti di una [[Variabili Aleatorie|v.a.]], 
Facciamo un esempio:

Siano $X_{1},\dots,X_{n}$ [[Variabili Aleatorie|v.a.]] [[IID]] [[Variabili Aleatorie Esponenziali|Esponenziali]] $Exp(\lambda)$ e $\lambda$ è incognito.

Per stimare $\lambda$ so innanzitutto che quando $n\gg1$ posso usare la formula:
$$\bar{X}=\dfrac{X_{1}+\dots+X_{n}}{n}\approx \mathbb{E}[X_{1}]=\dfrac{1}{\lambda}$$
Denotiamo quindi con $\hat{\lambda}_{mom}=\dfrac{1}{\bar{X}}$ il risultato della nostra stima con il metodo dei momenti.

Facciamo un altro esempio:
Siano $X_{1},\dots,X_{n}$ [[Variabili Aleatorie|v.a.]] [[IID]] [[Variabili Aleatorie Uniformi|uniformi]] $Unif(0,\theta)$.
Come prima, posso di