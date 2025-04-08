---
tags:
  - Probabilità_e_statistica
aliases:
  - v.a. di poisson
  - V.a. di Poisson
  - v.a. di Poisson
  - V.a. di poisson
  - poissoniane
---

>[!Definizione]  Definizione
>Le [[Variabili Aleatorie|v.a.]] di Poisson le usiamo per descrivere quanti eventi rari accadono in un intervallo di tempo fissato, ed ha le seguenti condizioni:
>- Un tasso $\lambda>0$ 
>$$X\sim Poi(\lambda)\quad \lambda>0$$
>La sua [[Fun. di massa di Probabilità (PMF)|PMF]] invece è tale che:
>$$f_{X}(x)=e^{-\lambda} \dfrac{\lambda^x}{x!}, \quad \forall x\in{0,1,2\dots}$$
>E allora l’ immagine sarà:
>$$\mathrm{Im}(X)=\mathbb{N}_{0}$$
>Ed invece il suo [[Valore Atteso]]:
>$$\mathbb{E}[X]=\lambda$$
>E la sua [[Varianza]]:
>$$Var(X)=\lambda$$


è interessante vedere che $Poi(\lambda)$ è il $\lim_{ n \to \infty }$ di $Bin(n, \dfrac{\lambda}{p})$, la possiamo allora vedere come un particolare tipo di [[Variabili Aleatorie Binomiali]]

Un’ altra interessante nozione è che la [[Variabili Aleatorie|v.a.]] di Poisson si dice “Chiusa rispetto la somma”, o anche la Riproducibilità, Ponendo che $X,Y$ siano [[Variabili Aleatorie Indipendenti|v.a. indipendenti]] allora possiamo definirla:
$$X+Y\sim Poi(\lambda_{1}+\lambda_{2})$$

E la [[Fun. di Ripartizione (CDF)|CDF]] sarà nella forma:
![[CDF Poisson.png]]