---
tags:
  - Probabilità_e_statistica
---
Ho un [[Campione Aleatorio]] con $n$ oggetti, dove ogni oggetto è difettoso indipendentemente dagli altri.

Come verifico le ipotesi:
- $H_{0}:p\leq p_{0}$
- $H_{1}:p>p_{0}$
*Dove p è la probabilità reale che un dato pezzo sia difettoso*

Allora svolgo come segue:

Sia $X$ il numero di pezzi difettosi nel campione

$$\mathbb{P}(X\geq k)=\sum^n_{i=k}\mathbb{P}(X=i)=\sum^n_{i=k}\binom{n}{i}p^i(1-p)^{n-1}$$
Allora cerchiamo la probabilità di avere più pezzi difettosi di un dato valore $k$.

Fissiamo un [[Livello di Significatività]] $\alpha\in(0,1)$ e quindi cerchiamo il $k$ minimo che rispetta questo livello.

$$K_{*}^\alpha=\min\left\{ k:\sum^n_{i=k}\binom{n}{i}p^i_{0}(1-p_{0})^{n-i} \right\}$$
Detto allora $x$ il numero di pezzi difettosi nel campione,
- Se $n\bar{x}<K_{*}^\alpha$ accetto $H_{0}$
- Altrimenti rifiuto.