---
tags:
  - Probabilità_e_statistica
---
Data una [[Regressione Lineare]], che segue la retta $Y=\alpha+\beta x+z$,

Un [[Intervalli di confidenza|IC]] al $(1-\gamma)100\%$ bilaterale per $\beta$ è dato da:
$$B\pm t_{\tfrac{\gamma}{2},n-2}\sqrt{ \dfrac{SS_{R}}{(n-2)S_{XX}} }$$
Per quanto riguarda invece la [[Verifica delle ipotesi]]:

$H_{0}:\beta=\beta_{0}$,
$H_{1}:\beta\neq \beta_{0}$

Se $H_{0}$ è vera allora la nostra [[Statistica Test]] sarà:

$$st=\sqrt{ \dfrac{S_{XX}(n-2) }{SS_{R}}}(\beta-\beta_{0})\sim t_{n-2}$$
Allora la [[p-value]]:
$$p-value:2\mathbb{P}(t_{n-2}>|st|\ )$$
E per un fissato [[Livello di Significatività]] $\gamma\in(0,1)$:
- Accetto $H_{0}$ se $|st|\leq t_{\tfrac{\gamma}{2},n-2}$
- Altrimenti rifiuto.

