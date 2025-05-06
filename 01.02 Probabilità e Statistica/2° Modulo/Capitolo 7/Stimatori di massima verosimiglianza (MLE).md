---
tags:
  - Probabilità_e_statistica
---
supponiamo di avere un [[Campione Aleatorio]] [[IID]] dove $X_{1},\dots,X_{n}$ sono [[Variabili Aleatorie Esponenziali|v.a. Esponenziali]] $Exp(\lambda)$, di media quindi $\dfrac{1}{\lambda}$, con $\lambda$ incognito.
Ricordiamoci quindi che la loro densità marginale è 
$$f(x)=\lambda e^{-\lambda x}$$
Pertanto, poiché le nostre [[Variabili Aleatorie|v.a.]] sono [[IID]], la loro distribuzione congiunta è data da:
$$f(x_{1},\dots,x_{n})=\prod^n_{i=1}\lambda e^{-\lambda x_{i}}$$
Qui usiamo una produttoria proprio perché le [[Variabili Aleatorie|v.a.]] sono [[IID]].

Allora creiamo la funzione di likelihood 