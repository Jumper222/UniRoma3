---
tags:
  - Probabilità_e_statistica
aliases:
  - Test Unilaterale
---

Vogliamo testare le ipotesi:
$H_{0}:\mu=\mu_{0}$
$H_{1}:\mu>\mu_{0}$

Ricordandoci che i valori della [[Statistica Test|Statistica Test]] $<\mu_{0}$ rafforzerebbero la “credibilità” di $H_{0}$ vs $H_{1}$

In questo caso stiamo parlando di Test Unilaterali, e la [[Regione Critica]] assumerà la forma:
$$C=\{\bar{x}>\mu_{0}+\dfrac{\sigma}{\sqrt{ n }}z_{\alpha}\}$$
*Per un valore di c in funzione della significatività desiderata*

In particolare per gli errori di <font color="#ffc000">prima specie</font>:

$c=(z_{\alpha}) \dfrac{\sigma}{\sqrt{ n }}$ dove $\alpha$ è la significatività che cerchiamo.

Per gli errori di <font color="#ffc000">seconda specie</font>:

$\beta(\mu)=\Phi\left(\dfrac{\sqrt{ n }}{\sigma}(\mu_{0}-\mu)+z_{\alpha}\right)$

Riassumendo:

1. Ho le ipotesi $H_{0}:\mu=\mu_{0}$, $H_{1}:\mu>\mu_{0}$, con una significatività $\alpha\in(0,1)$
	- Accetto $H_{0}$ se $\dfrac{\sqrt{ n }}{\sigma}(\bar{x}-\mu_{0})\leq z_{\alpha}$
	- Rifiuto $H_{0}$ altrimenti.
2. La [[p-value]] è $1-\Phi\left(\dfrac{\sqrt{ n }}{\sigma}(\bar{x}-\mu_{0})\right)$
3. La OC è: $\beta(\mu)=\Phi\left(\dfrac{\sqrt{ n }}{\sigma}(\mu-\mu_{0})-z_{\alpha}\right)$

Se invece avessimo $H_{1}:\mu<\mu_{0}$ allora useremmo le seguenti formule:

1. Ho le ipotesi $H_{0}:\mu=\mu_{0}$, $H_{1}:\mu<\mu_{0}$ con una significatività $\alpha\in(0,1)$
	- Accetto $H_{0}$ se $\dfrac{\sqrt{ n }}{\sigma}(\bar{x}-\mu_{0})\geq-z_{\alpha}$
	- Rifiuto $H_{0}$ altrimenti.
2. La [[p-value]] è $\Phi\left(\dfrac{\sqrt{ n }}{\sigma}(\bar{x}-\mu_{0})\right)$
3. La OC è: $\beta(\mu)=1-\Phi\left(\dfrac{\sqrt{ n }}{\sigma}(\mu-\mu_{0})-z_{\alpha}\right)$

