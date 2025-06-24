---
tags:
  - Probabilità_e_statistica
---

Dati due [[Campione Aleatorio|Campioni Aleatori]] normali $(X_{1},\dots,X_{n}),(Y_{1},\dots,Y_{n})$, con $\mu_{x},\mu_{y}$ ignoti, ma $\sigma^2_{x},\sigma^2_{y}$ noti:

Voglio testare:

$H_{0}:\mu_{x}=\mu_{y}$
$H_{1}:\mu_{x}\neq \mu_{y}$

Mi calcolo la [[Statistica Test]]:

$$st=\dfrac{\bar{x}-\bar{y}}{\sqrt{ \dfrac{\sigma^2_{x}}{n} +\dfrac{\sigma^2_{y}}{m}}}$$

#### <font color="#4bacc6">Verifica Bilaterale</font>



[[p-value]]:
$$2(1-\Phi(\ |st|\ ))$$
Fissato un $\alpha$:
- Accetto $H_{0}$ se $st<z_{\tfrac{\alpha}{2}}$
- Rifiuto altrimenti

#### <font color="#4bacc6">Verifica unilaterale destra</font>

$H_{0}:\mu_{x}=\mu_{y}$, $H_{1}:\mu _x>\mu_{y}$

[[p-value]]:
$$1-\Phi(st)$$
Fisso un $\alpha$:
- Accetto $H_{0}$ se $st< z_{\alpha}$
- Rifiuto altrimenti

#### Verifica unilaterale sinistra

$H_{0}:\mu_{x}=\mu_{y}$, $H_{1}:\mu _x<\mu_{y}$

[[p-value]]:
$$\Phi(st)$$
Fisso un $\alpha$:
- Accetto $H_{0}$ se $st> -z_{\alpha}$
- Rifiuto altrimenti
