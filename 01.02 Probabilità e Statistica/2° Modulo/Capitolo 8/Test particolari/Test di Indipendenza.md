---
tags:
  - Probabilità_e_statistica
---

Il test di Indipendenza lo usiamo per sapere se esiste una dipendenza di un qualche tipo tra i dati studiati, Quindi prende sempre in considerazione vettori di [[Variabili Aleatorie|v.a.]]

Facciamo un esempio:

![[Test di Indipendenza ESEMPIO.png]]

Abbiamo un campione $((x_{1},y_{1}),\dots,(x_{n},y_{n}))$
Dove $x_{i}\in\{\text{Donna, Uomo}\}=A$, $y_{i}\in\{\text{Dem,Rep,Ind}\}=B$

Allora chiamiamo due incognite $p_{a},q_{b}$, tali che:
- $p_{a}=\mathbb{P}(X_{i}=a)=\sum_{b\in B}\mathbb{P}(X_{i}=a,Y_{i}=b)$
- $q_{b}=\mathbb{P}(Y_{i}=b)=\sum_{a\in A}\mathbb{P}(X_{i}=a,Y_{i}=b)$
*Queste due v.a. ci serviranno poi per costruire l’ ipotesi $H_{0}$ di indipendenza*

