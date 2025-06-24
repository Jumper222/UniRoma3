---
tags:
  - Probabilità_e_statistica
---
Usiamo il Test T quando abbiamo un [[Campione Aleatorio]] normale e vogliamo verificare una ipotesi sulla media.
In questo caso però assumiamo che la [[Varianza]] $\sigma^2$ non sia nota.

Allora rimpiazziamo $\sigma$ con la [[Deviazione Standard Campionaria]]:
$$S=\sqrt{ \dfrac{1}{n-1}\sum^n_{i=1}(X_{i}-\bar{X} )^2}$$
Inoltre sappiamo che se il [[Campione Aleatorio]] è normale:
$$\dfrac{\sqrt{ n }}{S}(\bar{X}-\mu)=T\sim t_{n-1}$$
E questa sarà la nuova [[Statistica Test]].

#### <font color="#4bacc6">Test T bilaterale</font>

$H_{0}:\mu=\mu_{0}$
$H_{1}:\mu\neq \mu_{0}$

[[p-value]]: 
$$\mathbb{P}(\ |T_{n-1}|\ > \dfrac{\sqrt{ n }}{S}|\bar{x}-\mu_{0}|\ )=2\mathbb{P}(T_{n-1}\geq \dfrac{\sqrt{ n }}{S}|\bar{x}-\mu_{0}|\ )$$
Quindi per un fissato [[Livello di Significatività]] $\alpha$:

- Se $\dfrac{\sqrt{ n }}{S}|\bar{x}-\mu_{0}|\leq t_{\tfrac{\alpha}{2},n-1}$ allora accetto $H_{0}$
- Altrimenti rifiuto.