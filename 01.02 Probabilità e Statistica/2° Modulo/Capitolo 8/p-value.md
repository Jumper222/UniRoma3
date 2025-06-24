---
tags:
  - Probabilità_e_statistica
---
La p-value è il valore calcolato a partire dalla [[Statistica Test]] che ci dice, nel caso $H_{0}$ sia vera, quanto è probabile ottenere i dati che abbiamo campionato. 

Solitamente si usa assieme ad un [[Livello di Significatività]] $\alpha$, dove se è maggiore non rifiutiamo $H_{0}$, se è inferiore invece la rifiutiamo.

Per un <font color="#9bbb59">test bilaterale</font> la p-value è:
$$\mathbb{P}\left(\ |Z|>\dfrac{\bar{x}-\mu_{0}}{ \dfrac{\sigma}{\sqrt{ n }} }\right)$$
*Da notare come usiamo il valore assoluto di Z, questo proprio perché è un test bilaterale.*

Per un [[Test Unilaterali|Test Unilaterale]] invece la p-value sarà nella forma:
$$\mathbb{P}\left(\ Z>\dfrac{\bar{x}-\mu_{0}}{ \dfrac{\sigma}{\sqrt{ n }} }\right)$$
