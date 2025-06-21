---
tags:
  - Probabilità_e_statistica
aliases:
  - CLT
---

>[!Definizione]  Definizione
>Se $(X_{1},\dots,X_{n})$ è un [[Campione Aleatorio]] [[IID]] di dimensione infinita,
>Con $\mathbb{E}[X_{1}]=\mu$, $Var(X_{1})=\sigma^2<\infty$
>Allora
>$$\lim_{ n \to \infty }\mathbb{P}\left(\dfrac{\sqrt{ n }}{\sigma}(\bar{X}_{n}-\mu)\leq x\right) =\Phi(x) $$
>Ossia, è per $n\to \infty$ la distribuzione della [[Media Campionaria]] converge ad una [[Gaussiana Standard]] 

Il succo del CLT è che per un campione con [[Variabili Aleatorie|v.a.]] qualsiasi, con valore atteso $\mu$ e varianza $\sigma^2<\infty$ sufficientemente grande, esso sarà sempre approssimabile ad una [[Gaussiana Standard]]. 