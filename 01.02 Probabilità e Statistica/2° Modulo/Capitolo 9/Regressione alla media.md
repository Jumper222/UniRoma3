---
tags:
  - Probabilità_e_statistica
---
La Regressione alla media è un fenomeno di relazione lineare tra input e output del tipo:
$$Y=\alpha+\beta x+Z$$
Dove $\beta\in(0,1)$

Questo quindi ci porta a:
- $\mathbb{E}[Y]<x$ se $x$ è molto grande
- $\mathbb{E}[Y]>x$ se $x$ è molto piccolo

*Concettualmente questo significa che in un campione stanno avvenendo tanti valori “fuori scala“, allora ci aspettiamo che il prossimo valore torni più vicino alla media, bilanciandosi rispetto agli altri valori.*

Ciò significa che se stiamo studiando una regressione alla media avremo [[Intervalli di confidenza|IC]]:
$$IC_{\gamma}:A\pm t_{\tfrac{\gamma}{2},n-2}\sqrt{ \dfrac{SS_{R}\sum^n_{i=1}x^2_{i}}{n(n-2)S_{XX}} }$$
Invece la [[Statistica Test]] per $H_{0}:\alpha=\alpha_{0}$ ([[Test T]])

$$\sqrt{ \dfrac{n(n-2)S_{XX}}{SS_{R}\sum^n_{i=1}x^2_{i}} }|A-\alpha_{0}|$$ *se $H_{1}:\alpha\neq\alpha_{0}$*
oppure $$\sqrt{ \dfrac{n(n-2)S_{XX}}{SS_{R}\sum^n_{i=1}x^2_{i}} }(A-\alpha_{0})$$
se $H_{1}:\alpha>\alpha_{0}$ o $H_{1}:\alpha<\alpha_{0}$

