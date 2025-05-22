---
tags:
  - Probabilità_e_statistica
---
Il metodo di [[Stima Parametrica]] usando gli Stimatori Bayesani si basa sull’ effettuare una stima per $\theta$, conoscendo oltre alla distribuzione, anche delle informazioni a priori su come è distribuito $\pi(\theta)$.
Ciò significa che avremo un $\theta$ che invece di essere un numero sarà un’ <font color="#9bbb59">intervallo</font>, che poi andremo a calcolare se ci fa perdere informazioni o meno con una <font color="#ffc000">Loss function</font> 

> [!definizione]  Definizione
> Dati un [[Campione Aleatorio]] $(x_{1},\dots,x_{n})$ di [[Variabili Aleatorie|v.a.]] [[IID]], ed una funzione [[Fun. di densità di Probabilità (PDF)|PDF]] o [[Fun. di massa di Probabilità (PMF)|PMF]] $f(x\ |\ \theta)$, 