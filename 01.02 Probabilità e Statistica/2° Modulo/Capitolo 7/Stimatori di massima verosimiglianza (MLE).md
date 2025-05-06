---
tags:
  - Probabilità_e_statistica
---
supponiamo di avere un [[Campione Aleatorio]] [[IID]] dove $X_{1},\dots,X_{n}$ sono [[Variabili Aleatorie Esponenziali|v.a. Esponenziali]] $Exp(\lambda)$, di media quindi $\dfrac{1}{\lambda}$, con $\lambda$ incognito.
Ricordiamoci quindi che la loro densità marginale è 
$$f(x)=\lambda e^{-\lambda x}$$
Pertanto, poiché le nostre [[Variabili Aleatorie|v.a.]] sono [[IID]], la loro distribuzione congiunta è data da:
$$f(x_{1},\dots,x_{n})=\prod^n_{i=1}\lambda e^{-\lambda x_{i}}$$
Qui usiamo una produttoria proprio perché le [[Variabili Aleatorie|v.a.]] sono [[IID]].

Allora creiamo la funzione di likelyhood:
$$L(\theta)=\prod^n_{i=1}\lambda e^{-\lambda x_{i}}$$
Quindi usiamo il suo $\log$, e poi deriviamo.
Allora calcoliamo il massimo:
$$\dfrac{d\ln L(\theta)}{dt}$$
Facciamo un esempio:

Sia $(x_{1},\dots,x_{n})$ un [[Campione Aleatorio]] [[IID]] di [[Variabili Aleatorie di Bernoulli|bernoulliane]] $Bern(p)$
Allora per l’MLE di p dovremmo:
$$f(x_{1},\dots,x_{n}|p)=p^{\sum^n_{i=1}x_{i}}(1-p)^{n-\sum ^n_{i=1}x_{i}}$$
Questa è la [[Fun. di Ripartizione (CDF)|CDF]] del campione aleatorio, ora applichiamo $\ln$:
$$\ln f(x_{1},\dots,x_{n}|p)=\left( \sum^n_{i=1}x_{i} \right)\ln(p)+\left( n-\sum^n_{i=1}x_{i} \right)\ln(1-p)$$
Ora deriviamo:
$$\dfrac{d}{dp}\ln f(x_{1},\dots,x_{n}|p)=\dfrac{1}{p}\sum^n_{i=1}x_{i}-\dfrac{1}{1-p}\left( n-\sum^n_{i=1}x_{i} \right)$$
Ora lo poniamo uguale a $0$, e adesso ricordandoci che $p\in(0,1)$
$$\dfrac{1}{p}\sum^n_{i=1}x_{i}-\dfrac{1}{1-p}\left( n-\sum^n_{i=1}x_{i} \right)=0$$
E infine

![[Esempio MLE Bernoulli.png]]

Possiamo allora dire che per una [[Variabili Aleatorie di Bernoulli|bernoulliana]] il MLE sarà uguale a $\bar{x}$, in notazione scriviamo:
$$\hat{p}_{MLE}=\bar{x}$$