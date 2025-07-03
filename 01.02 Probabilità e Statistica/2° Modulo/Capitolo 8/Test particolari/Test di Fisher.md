---
tags:
  - Probabilità_e_statistica
---

Dati 2 [[Campione Aleatorio|Campioni Aleatori]] $(x_{1},\dots,x_{n}),(y_{1},\dots,y_{m})$
Possiamo creare una tabella di contingenza, dove incrociamo predizione e realtà. quindi andiamo a vedere quante volte la predizione ha preso la realtà (nella tabella è $x$) e quante volte si è sbagliata ($y$)
quindi andiamo a sottrarre dal campione studiato e creiamo la tabella.

|            | Predizione = 1 | Predizione = 0 |
| ---------- | -------------- | -------------- |
| Realtà = 1 | $x$            | $n-x$          |
| Realtà = 2 | $y$            | $m-x$          |
Dove $\ell=x+y$

Quindi creo le ipotesi $H_{0},H_{1}$:
$H_{0}:$ Le due [[Variabili Aleatorie]] sono indipendenti, la predizione non rispecchia la realtà.
$H_{1}:$ La predizione rispecchia la realtà.
        
Trovo allora la [[Statistica Test]]:

$$\mathbb{P}(X=k|\ell)=\dfrac{\binom{n}{k}\binom{m}{\ell-k}}{\binom{N}{\ell}}$$
    
