---
tags:
  - Probabilità_e_statistica
aliases:
  - v.a. Binomiali
  - V.a. binomiali
  - v.a. binomiali
---
 
>[!Definizione]  Definizione
>La [[Variabili Aleatorie|v.a.]] binomiale $X\sim Bin(n,p)$
>Si utilizza quando si vuole <font color="#4bacc6">contare il numero di successi</font> in un numero $n$ di prove indipendenti, ognuna delle quali può “<font color="#9bbb59">Succedere</font>” o “<font color="#c0504d">Fallire</font>”, è quindi utile per studiare una serie di [[Variabili Aleatorie di Bernoulli|bernoulliane]],
>Allora abbiamo:
>
>- $n$ numero totale di prove
>- $p$ probabilità costante per ogni prova
>- il numero di successi $k$ in $n$ prove
>
>Quindi abbiamo [[Fun. di massa di Probabilità (PMF)|PMF]]:
>$$P(X=k)=\binom{n}{k}p^k(1-p)^{n-k}$$
>[[Valore Atteso]]:
>$$\mathbb{E}[X]=np$$
>Momento secondo:
>$$\mathbb{E}[X^2]=np(1-p)+(np)^2$$
>[[Varianza]]:
>$$np(1-p)$$
>[[Funzione generatrice di momenti (MGF)|MGF]]
>$$M_{X}(t)=(1-p+pe^t)^n$$

Il grafico [[Fun. di massa di Probabilità (PMF)|PMF]] di una [[Variabili Aleatorie|v.a.]] binomiale è:
![[CDF Binomiale.png]]