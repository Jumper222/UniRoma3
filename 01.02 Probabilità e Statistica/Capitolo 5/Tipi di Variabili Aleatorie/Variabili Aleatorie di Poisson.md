#Probabilità_e_statistica 
>[!Definizione]  Definizione
>Una [[Variabili Aleatorie|v.a.]] ci serve per poter definire meglio la possibilità che avvengano eventi “rari” ed è scritta tale che:
>$$X\sim Poi(\lambda)\quad \lambda>0$$
>La sua [[Fun. di Ripartizione (CDF)]] invece è tale che:
>$$f_{X}(x)=e^{-\lambda} \dfrac{\lambda^x}{x!}, \quad \forall x\in{0,1,2\dots}$$
>E allora l’ immagine sarà:
>$$\mathrm{Im}(X)=\mathbb{N}_{0}$$
>Ed invece il suo [[Valore Atteso]]:
>$$mathbb{E}[X]=\lambda$$
>E la sua [[Varianza]]:
>$$Var(X)=\lambda$$
>è interessante vedere che $Poi(\lambda)$ è il $\lim_{ n \to \infty }$ di $Bin(n, \dfrac{\lambda}{p})$, la possiamo allora vedere come un particolare tipo di [[Variabili Aleatorie Binomiali]]