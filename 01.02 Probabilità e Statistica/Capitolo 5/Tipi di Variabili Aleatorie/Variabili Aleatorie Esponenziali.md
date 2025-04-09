---
tags:
  - Probabilità_e_statistica
aliases:
  - v.a. Esponenziali
  - V.a. esponenziali
  - v.a. esponenziali
  - V.a. Esponenziali
---

>[!Definizione]  Definizione
>$X\sim Exp(\lambda)$
>Una [[Variabili Aleatorie|v.a.]] Esponenziale è un tipo di [[Variabili Aleatorie discrete e continue|v.a. continua]] utile per i [[Processi di Bernoulli e Poisson]], deve avere un tasso ($\lambda$) o intensità ed è tale che:
>[[Fun. di densità di Probabilità (PDF)|PDF]]: $f_{X}(x)=\lambda e^{-\lambda x}$
>[[Valore Atteso]]: $\mathbb{E}[X]=\dfrac{1}{\lambda}$
>[[Varianza]]: $Var(X)=\dfrac{1}{\lambda^2}$
>[[Funzione generatrice di momenti (MGF)|MGF]]: $M_{X}(t)=\dfrac{\lambda}{\lambda-t}$
>
>##### Proprietà
>è Memoryless, ossia la probabilità non tiene conto del tempo già passato
>Se $Y=cX$, $X\sim Exp(\lambda)$, allora $Y\sim Exp(\dfrac{\lambda}{c})$ 

Graficamente sarà nella forma:
![[Variabili Aleatorie Esponenziali.png]]
La [[Fun. di Ripartizione (CDF)|CDF]] invece:
$$\mathbb{P}(X>x)=e^{-\lambda x}$$
![[Variabili Aleatorie Esponenziali 2.png]]
Possiamo vedere le v.a. Esponenziali come [[Variabili Aleatorie Geometriche|v.a. Geometriche]] con $n$ che tende a 0, e prob. di successo infinitesima

E allora visto che derivano dalle [[Variabili Aleatorie Geometriche|v.a. Geometriche]], anche le Esponenziali hanno la proprietà dell’ assenza di memoria.

Altre proprietà includono:

- Chiusura rispetto al minimo
	Con $n$ [[Variabili Aleatorie Indipendenti|v.a. indipendenti]], se le uniamo in una sola v.a. $Y$, anch’essa sarà esponenziale:
	$$Y=min\{X_{1},X_{2},\dots,X_{n}\}\sim Exp\left( \sum_{i=1}^n \right)$$
- Proprietà delle costanti
	Se $X\sim Exp(\lambda)$, se prendiamo una costante $c>0$, t.c $Y=cX$, allora:
	$$Y\sim Exp(\dfrac{\lambda}{c})$$
	
	