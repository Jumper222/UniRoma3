---
tags:
  - Probabilità_e_statistica
---
Grazie al [[Teorema del Limite Centrale (CLT)]], possiamo dire che le [[Variabili Aleatorie Binomiali|v.a. Binomiali]] sono approssimabili come:

Se $Y_{n}\sim Bin(n,p)$

Se $\lim_{ n \to \infty }np=\lambda \in(0,\infty)$ avremo che $Y_{n}\sim Poi(\lambda)$
Se $\lim_{ n \to \infty }np=\infty$ allora avremo che $Y_{n}\sim \mathcal{N}(pn,np(1-p))$

##### Binomiale in Normale

Se abbiamo una [[Variabili Aleatorie Binomiali|v.a. Binomiale]] $X\sim Bin(n,p)$, con $np\gg 1$
Allora possiamo trasformarla in [[Gaussiana Standard]] t.c:
$$\mathbb{P} \left(\dfrac{X-np}{\sqrt{ np(1-p) }}\leq x\right)\sim\mathbb{P}(Z\leq x)$$ E questa è proprio la distribuzione normale!