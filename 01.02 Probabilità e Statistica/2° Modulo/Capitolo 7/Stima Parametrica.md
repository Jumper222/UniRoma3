---
tags:
  - Probabilità_e_statistica
---
Una stima parametrica è un problema in cui siamo interessati a conoscere il valore del parametro che regola la [[Variabili Aleatorie|v.a.]]:
Abbiamo un [[Campione Aleatorio]] [[IID]] con [[Fun. di Ripartizione (CDF)|CDF]] $F(\cdot|\theta)$
Il nostro obiettivo è stimare $\theta$.

Esistono 4 metodi per stimare $\theta$:


##### [[Metodo di Momenti]]
Usiamo i momenti campionari (e la [[Legge debole dei grandi numeri|LDGN]]) per stimare i momenti teorici

##### [[Stimatori di massima verosimiglianza (MLE)]]
Produciamo una stima puntuale di $\theta$ risolvendo un problema di ottimizzazione

##### [[Intervalli di confidenza]]
Produciamo una stima di un intervallo $I\subset\mathbb{R}$ e di un valore $z\in(0,1)$ t.c. $\mathbb{P}(\theta\in I)>z$, usando il [[Teorema del Limite Centrale (CLT)|CLT]]

##### [[Stimatori Bayesani]]
Produciamo una stima puntuale per $\theta$ utilizzando oltre al [[Campione Aleatorio]] $X_{1},\dots,X_{n}$ anche informazioni aggiuntive su $\theta$ a prori