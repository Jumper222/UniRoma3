#Probabilità_e_statistica 
>[!Definizione]  Definizione
>La Disuguaglianza di Chebyshev è simile a quella di [[Disuguaglianza di Markov|Markov]], però prende in considerazione anche la [[Varianza]], dando molte volte una stima più accurata:
>$$\mathbb{P}(|X-\mathbb{E}[X]|\geq r)\leq \dfrac{\sigma^2}{r^2}$$
>L’ unico requisito è che $r>\sigma$

Inoltre possiamo dire che la probabilità che $X$ si discosti dalla sua media più di k-volte la sua [[Deviazione Standard]] è al più $\dfrac{1}{k^2}$, scegliendo $r=k\sigma$ abbiamo:
$$\mathbb{P}(|X-\mathbb{E}[X]|\geq k\sigma) \leq \dfrac{\sigma^2}{k^2\sigma^2}=\dfrac{1}{k^2}$$