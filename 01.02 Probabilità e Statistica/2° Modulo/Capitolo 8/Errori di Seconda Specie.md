---
tags:
  - Probabilità_e_statistica
---
Negli esercizi degli Errori di Seconda Specie andiamo a studiare la probabilità di accettare o rifiutare $H_{0}$ quando è incorretta.


Abbiamo la [[Funzioni|Funzione]] <font color="#f79646">OC</font> (Operating Charateristic), se $\mu$ è vera:
$$\beta(\mu)=\Phi(z_{\dfrac{\alpha}{2}}+\dfrac{\sqrt{ n }}{\sigma}(\mu_{0}-\mu))-\Phi(-z_{\dfrac{\alpha}{2}}+\dfrac{\sqrt{ n }}{\sigma}(\mu_{0}-\mu))$$
1. $1-\beta(\mu)$ è detta potenza del test.

La funzione OC rappresenta la probabilità di accettare $H_{0}$ quando $\mu=\mu_{1}$, ossia $H_{0}$ è falsa.
Noi vogliamo che questa probabilità sia minore di un valore dato $\delta$.
Allora il nostro obiettivo sarà trovare un numero $n$ rappresentante la numerosità minima del campione per poter far valere l’ equazione $\beta(\mu_{1})<\delta$


Se abbiamo $\mu=\mu_{1}$ (e il [[Livello di Significatività]] è fissato ad $\alpha$), ed un parametro dato $\delta$ allora voglio un campione con numerosità:
$$n>\left[\dfrac{(z_{\dfrac{\alpha}{2}}+z_{\delta})\sigma}{\mu_{1}-\mu_{0}}\right]^2$$