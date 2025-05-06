---
tags:
  - Probabilità_e_statistica
---

Poniamo che abbiamo un [[Campione Aleatorio]]  $(X_{1},\dots,X_{n})$ [[IID]] [[Variabili Aleatorie di Bernoulli|bernoulliane]] $Bern(p)$

Abbiamo Alice, che conosce tutto il campione
Poi c’è Bob, che conosce solo $\bar{X}$ (ed $n$)
Chi ha più informazioni?

L’ informazione è la stessa!
Bob può generare un campione $Y_{1},\dots,Y_{n}$ t.c. $\bar{Y}=\bar{X}$
E allora $f(Y_{1},\dots,Y_{n}|p)=f(X_{1},\dots,X_{n}|p)$
Allora possiamo dire che $\bar{X}$ contiene tutte le info necessarie a stimare $\theta$

Allora $\bar{X}$ si dice una <font color="#f79646">statistica sufficiente</font>.