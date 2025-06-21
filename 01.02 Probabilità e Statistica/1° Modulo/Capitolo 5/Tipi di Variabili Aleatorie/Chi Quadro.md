---
tags:
  - Probabilità_e_statistica
aliases:
  - Chi quadrato
  - chi-quadrato
  - Chi-quadrato
  - chi quadro
---

>[!Definizione]  Definizione
>Il Chi-Quadrato (o quadro), indicato con $\chi$ è una famiglia di distribuzioni di probabilità [[Variabili Aleatorie discrete e continue|continua]] che dipende da un parametro di gradi dii libertà $k$.
>Queste distribuzioni si ottengono sommando tra loro i quadrati di k [[Gaussiana Standard|Gaussiane standard]], ossia [[Variabili Aleatorie Gaussiane|v.a. Gaussiane]] con [[Valore Atteso]] = 0 e [[Varianza]] = 1.
>Allora Chi-Quadro è definito tale che:
>$$\chi^2=Z^2_{1}+Z^2_{2}+\dots+Z^2_{k}$$
>Allora avremo che il [[Valore Atteso]]:
>$$\mathbb{E}[\chi]=k$$
>E la [[Varianza]]:
>$$Var(\chi)=2k$$
### <font color="#4bacc6">Proprietà di Chi Quadro</font>

Esattamente come le [[Variabili Aleatorie Gaussiane|v.a. Gaussiane]], anche Chi Quadro è riproducibile, ossia:

Se $X\sim\chi^2_{n}$ e $Y\sim\chi^2_{m}$, indipendenti, allora
$$X+Y\sim \chi^2_{n+m}$$
Un’ altra utile proprietà è che la distribuzione Chi Quadro è sempre non negativa, ed all’ aumentare dei gradi di libertà $k$ diventa sempre più simmetrica (<font color="#ffff00">asimmetrica</font> a destra per $k$ piccoli e quasi <font color="#ffff00">simmetrica</font> per $k$ grandi)

Esattamente come per le [[Variabili Aleatorie Gaussiane|v.a. Gaussiane]], anche per Chi Quadro possiamo studiare il [[Punto Critico Chi Quadro]]

### <font color="#4bacc6">Approssimazione ad una Gaussiana</font>

Come detto in precedenza, per $k$ grande converge ad una [[Variabili Aleatorie Gaussiane|v.a. gaussiana]] con media $k$ e varianza $2k$
Per portarla ad una [[Gaussiana Standard]] possiamo usare la formula:
$$\dfrac{\chi-k}{\sqrt{ 2k }}\approx\mathcal{N}(0,1)$$

### <font color="#4bacc6">PDF di Chi Quadro</font>

![[PDF Chi Quadro.png]]