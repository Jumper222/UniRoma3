---
tags:
  - Probabilità_e_statistica
---
Ho due popolazioni di [[Variabili Aleatorie di Bernoulli|bernoulliane]]: $Bern(p),Bern(q)$,
Con [[Campione Aleatorio|Campioni]]: $(x_{1},\dots,x_{n})$,$(y_{1},\dots,y_{m})$

Come testo se $p\neq q$ ?

Facciamo un esempio:

Prendiamo due linee di produzione:

- Linea 1: $(X_{1},\dots,X_{n})$ [[IID]] $Bern(p)$
- Linea 2: $(Y_{1},\dots,Y_{n})$ [[IID]] $Bern(q)$

Chiamo $X_{tot}=\sum^n_{i=1}X_{i}$, $Y_{tot}=\sum^m_{i=1}Y_{i}$

Se $H_{0}$ è vera, ossia $p=q$ allora
$X_{tot}+Y_{tot}\sim bin(n+m,p)$

Facciamo finta di prendere pezzi a caso da queste linee di produzione, la prima li fa rossi e la seconda blu.

Possiamo sempre dire allora che la probabilità di estrarre $k$ rosse è:
$$\mathbb{P}(X_{tot}=k\ | X_{tot}+Y_{tot}=l )=\dfrac{\binom{n}{k}\binom{m}{l-k}}{\binom{n+m}{l}}$$
*Senza reinserimento!*

Allora calcolo $x_{tot}$ e $y_{tot}$ *Semplicemente il numero totale di campioni di x e y*
ed anche $l=x_{tot}+y_{tot}$

Posso allora fissare un [[Livello di Significatività]] $\alpha$, ed avere due situazioni:

Se:
$$\sum^{x_{tot}}_{k=0}\dfrac{\binom{n}{k}\binom{m}{l-k}}{\binom{n+m}{l}}\leq \alpha$$
Oppure se:
$$\sum^l_{k=x_{tot}}\dfrac{\binom{n}{k}\binom{m}{l-k}}{\binom{n+m}{l}}\leq \alpha$$

Allora rifiuterò $H_{0}$

Allora la [[p-value]] è il minimo tra i due, formalizzato:
$$p-value=\min\left\{\sum^{x_{tot}}_{k=0}\dfrac{\binom{n}{k}\binom{m}{l-k}}{\binom{n+m}{l}},\sum^l_{k=x_{tot}}\dfrac{\binom{n}{k}\binom{m}{l-k}}{\binom{n+m}{l}} \right\}$$