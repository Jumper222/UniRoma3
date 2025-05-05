---
tags:
  - Probabilità_e_statistica
aliases:
  - T
  - student
---

>[!definizione]  Definizione
>$\forall m\geq 1$  diciamo che T è una [[Variabili Aleatorie|v.a.]] con $m$ gradi di libertà, $T\sim t_{m}$
>Allora $T$ può essere espresso come il rapporto:
>$$T=\dfrac{Z}{\sqrt{ \dfrac{C}{m} }}$$
>Dove $Z\sim \mathcal{N}(0,1)$ ossia [[Gaussiana Standard|Distribuzione Normale]]
>e $C\sim\mathcal{X}^2_{m}$, ossia una [[Chi Quadro]]
>
>Per il [[Valore Atteso]] abbiamo la formula:
>$$\mathbb{E}[T]=0$$
>e la [[Varianza]]:
>$$\dfrac{m}{m-2}$$ 

Per la [[Legge debole dei grandi numeri]] abbiamo che più $m$ aumenta e più T assomiglia di più a $\mathcal{N}(0,1)$

In conclusione possiamo dire che:
$$\dfrac{\sqrt{ n }}{S}(\bar{X}-\mu)s$$