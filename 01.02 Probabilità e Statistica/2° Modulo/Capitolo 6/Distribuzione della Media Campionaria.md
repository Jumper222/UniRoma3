---
tags:
  - Probabilità_e_statistica
---

La più semplice [[Statistica]] a cui si può pensare è la [[Media Campionaria]] di un [[Campione Aleatorio]] $(X_{1},\dots,X_{n})$:
$$\bar{X}=\dfrac{X_{1}+\dots+X_{n}}{n}$$
*in questo caso $\bar{X}$ è una [[Variabili Aleatorie|v.a.]]*

Ci domandiamo quindi quanto vale il [[Valore Atteso]] e la [[Varianza]] di $\bar{X}$:

Il [[Valore Atteso]] sarà uguale a $\mathbb{E}[X_{1}]$, questo per via della proprietà di IID.
La [[Varianza]] invece sarà:
$Var\left( \dfrac{1}{n}\sum^n_{i=1}X_{i} \right)=\dfrac{1}{n^2}Var\left( \sum^n_{i=1} X_{i} \right)=\dfrac{1}{n^2}nVar(X_{1})=\dfrac{Var(X_{1})}{n}$
Questo avviene per la proprietà della varianza [[Calcolare la varianza di una funzione]], dove la costante moltiplicativa  quando esce dalla varianza diventa $^2$

Questo deriva dalla [[Legge debole dei grandi numeri]], che ci dice che per un [[Campione Aleatorio]] di grandezza $n$ che tende ad infinito, allora $\bar{X}_{n}$ è asintoticamente deterministica, e coincide con il valore atteso di un elemento del campione. 

Se volessimo fare di meglio, ricorreremmo al [[Teorema del Limite Centrale (CLT)]]
