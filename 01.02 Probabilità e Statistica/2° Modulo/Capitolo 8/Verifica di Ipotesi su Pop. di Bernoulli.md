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

$$\mathbb{P}(X\geq k)=\sum^n_{i=k}\mathbb{P}(X=i)=\sum^n_{i=k}\binom{n}{i}p^i(1-p)$$