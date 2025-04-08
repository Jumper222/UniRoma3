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
>Una [[Variabili Aleatorie|v.a.]] Esponenziale è un tipo di [[Variabili Aleatorie discrete e continue|v.a. continua]] utile per i [[Processi di Bernoulli e Poisson]], ed è tale che:
>$$f_{X}(x)=\lambda e^{-\lambda x}$$
>e si scrive:
>$$X\sim Exp(\lambda)$$
>Questo lambda lo chiamiamo <font color="#9bbb59">Intensità</font>, <font color="#9bbb59">rate</font> o <font color="#9bbb59">tasso</font>
>Graficamente sarà nella forma:
>
>![[Variabili Aleatorie Esponenziali.png]]
>La [[Fun. di Ripartizione (CDF)|CDF]] invece:
>$$\mathbb{P}(X>x)=e^{-\lambda x}$$
>![[Variabili Aleatorie Esponenziali 2.png]]
>
>Allora il [[Valore Atteso]] sarà:
>$$\dfrac{1}{\lambda}$$
>E la [[Varianza]]:
>$$\dfrac{1}{\lambda^2}$$


Possiamo vedere le v.a. Esponenziali come [[Variabili Aleatorie Geometriche|v.a. Geometriche]] con $n$ che tende a 0, e prob. di successo infinitesima

E allora visto che derivano dalle [[Variabili Aleatorie Geometriche|v.a. Geometriche]], anche le Esponenziali hanno la proprietà dell’ assenza di memoria.

Altre proprietà includono:

- Chiusura rispetto al minimo
	Con $n$ [[Variabili Aleatorie Indipendenti|v.a. indipendenti]], se le uniamo in una sola v.a. $Y$, anch’essa sarà esponenziale:
	$$Y=min\{X_{1},X_{2},\dots,X_{n}\}\sim Exp\left( \sum_{i=1}^n \right)$$
- Proprietà delle costanti
	Se $X\sim Exp(\lambda)$, se prendiamo una costante $c>0$, t.c $Y=cX$, allora:
	$$Y\sim Exp(\dfrac{\lambda}{c})$$
	
	