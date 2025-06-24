---
tags:
  - Probabilità_e_statistica
---

Vogliamo testare le ipotesi:
$H_{0}:\mu=\mu_{0}$
$H_{1}:\mu>\mu_{0}$

Ricordandoci che i valori della [[p-value e Statistica Test|Statistica Test]] $<\mu_{0}$ rafforzerebbero la “credibilità” di $H_{0}$ vs $H_{1}$

In questo caso stiamo parlando di Test Unilaterali, e la [[Regione Critica]] assumerà la forma:
$$C=\{(x_{1},\dots ,x_{n})\in \mathbb{R}^n|\ \bar{x}-\mu>c\}$$
*Per un valore di c in funzione della significatività desiderata*

In particolare per gli errori di <font color="#ffc000">prima specie</font>:

$c=(z_{\alpha}) \dfrac{\sigma}{\sqrt{ n }}$ dove $\alpha$ è la significatività che cerchiamo.

Per gli errori di <font color="#ffc000">seconda specie</font>:

$\beta(\mu)=\Phi(\dfrac{\sqrt{ n }}{\sigma})$