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

Guardiamo il campione e chiamiamo:
$$N_{a,b}=\sum^n_{i=1}\mathbb{1}(X_{i}=a,Y_{i}=b)$$
*Ossia quante volte appaiono i valori in tabella.*

$M_{a}=\sum_{b\in B}N_{a,b}$ *Quanta gente è uomo o donna*
$R_{b}=\sum_{a\in A}N_{a,b}$ *Quanta gente ha votato un partito*

Uno stimatore è dato da:

$\hat{p}_{a}=\dfrac{M_{a}}{n}$
$\hat{q}_{b}=\dfrac{R_{b}}{n}$

Se genere e appartenenza politica fossero indipendenti allora avremmo:
$N_{a,b}\approx \hat{p}_{a}\hat{q}_{b}n$

Posso finalmente creare le ipotesi: 
$H_{0}:\mathbb{P}(X=a,Y=b)=p_{a}q_{b}$
$H_{1}:\mathbb{P}(X=a,Y=b)\neq p_{a}q_{b}$

Allora la nostra [[Statistica Test]] sarà:

$$$$