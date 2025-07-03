---
tags:
  - Probabilità_e_statistica
---
Dati due [[Campione Aleatorio|Campioni Aleatori]] normali $(X_{1},\dots,X_{n}),(Y_{1},\dots,Y_{n})$, con $\mu_{x},\mu_{y}$ ignoti, $\sigma$ uguale ma ignota

Sfrutto lo Stimatore Pooled, già visto con gli [[Intervalli di confidenza]]:

$$S_{p}^2=\dfrac{(n-1)S^2_{x}+(m-1)S^2_{y}}{n+m-2}$$

La [[Statistica Test]] allora sarà data da:

$$st= \dfrac{\bar{x}-\bar{y}}{S_{p}\left(\dfrac{1}{n}+\dfrac{1}{m}\right)}$$

#### <font color="#4bacc6">Test bilaterale</font>

[[p-value]]:
$$2\mathbb{P}(T>|st|\ )$$ *Con T avente n+m-2 gradi di libertà*

Fisso un $\alpha$:
- Accetto $H_{0}$ se $|st|\leq t_{n+m-2, \tfrac{\alpha}{2}}$
- Rifiuto altrimenti.

#### <font color="#4bacc6">Test unilaterale da destra</font>

[[p-value]]:
$$\mathbb{P}(T>st )$$ *Con T avente n-m-2 gradi di libertà*

Fisso un $\alpha$:
- Accetto $H_{0}$ se $st\leq t_{n+m-2,\alpha}$
- Rifiuto altrimenti.

#### Test unilaterale da sinistra

[[p-value]]:
$$\mathbb{P}(T<st )$$ *Con T avente n-m-2 gradi di libertà*

Fisso un $\alpha$:
- Accetto $H_{0}$ se $st\geq -t_{n+m-2,\alpha}$
- Rifiuto altrimenti.