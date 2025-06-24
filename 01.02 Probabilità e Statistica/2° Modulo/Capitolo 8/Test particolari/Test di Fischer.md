---
tags:
  - Probabilità_e_statistica
---
Ho due popolazioni di [[Variabili Aleatorie di Bernoulli|bernoulliane]]: $Bern(p),Bern(q)$,
Con [[Campione Aleatorio|Campioni]]: $(x_{1},\dots,x_{n})$,$(y_{1},\dots,y_{n})$

Come testo se $p\neq q$ ?

Facciamo un esempio:

Prendiamo due linee di produzione:

- Linea 1: $(X_{1},\dots,X_{n})$ [[IID]] $Bern(p)$
- Linea 2: $(Y_{1},\dots,Y_{n})$ [[IID]] $Bern(q)$

Chiamo $X_{tot}=\sum^n_{i=1}X_{i}$, $Y_{tot}=\sum^n_{i=1}Y_{i}$

Se $H_{0}$ è vera, ossia $p=q$ allora
$X_{tot}+Y_{tot}\sim bin(n+m,p)$

Facciamo finta di prendere pezzi a caso da queste linee di produzione, la prima li fa rossi e la seconda blu.

Possiamo sempre dire allora ch