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
>Le [[Variabili Aleatorie|v.a.]] di Poisson le usiamo per descrivere quanti eventi accadono in un intervallo di tempo fissato, differisce dalle [[Variabili Aleatorie Binomiali|v.a. binomiali]] in quanto è più approssima più correttamente eventi rari su intervalli piccoli, ed ha le seguenti condizioni:
>- Gli eventi sono indipendenti tra loro
>- La probabilità è costante
>- Il numero medio di questi eventi nell’ intervallo è noto
>
>La sua [[Fun. di massa di Probabilità (PMF)|PMF]] invece è tale che:
>$$f_{X}(x)=e^{-\lambda} \dfrac{\lambda^x}{x!}, \quad \forall x\in{0,1,2\dots}$$
>Ed invece il suo [[Valore Atteso]]:
>$$\mathbb{E}[X]=\lambda$$
>Il suo momento secondo:
>$$\mathbb{E}[X^2]=\lambda+\lambda^2$$
>E la sua [[Varianza]]:
>$$Var(X)=\lambda$$
>La sua [[Funzione generatrice di momenti (MGF)|MGF]]:
>$$M_{x}(t)=e^{\lambda(e^t-1)}$$


è interessante vedere che $Poi(\lambda)$ è il $\lim_{ n \to \infty }$ di $Bin(n, \dfrac{\lambda}{p})$, la possiamo allora vedere come un particolare tipo di [[Variabili Aleatorie Binomiali]]

Un’ altra interessante nozione è che la [[Variabili Aleatorie|v.a.]] di Poisson si dice “Chiusa rispetto la somma”, o anche la Riproducibilità, Ponendo che $X,Y$ siano [[Variabili Aleatorie Indipendenti|v.a. indipendenti]] allora possiamo definirla:
$$X+Y\sim Poi(\lambda_{1}+\lambda_{2})$$

E la [[Fun. di Ripartizione (CDF)|CDF]] sarà nella forma:
![[CDF Poisson.png]]