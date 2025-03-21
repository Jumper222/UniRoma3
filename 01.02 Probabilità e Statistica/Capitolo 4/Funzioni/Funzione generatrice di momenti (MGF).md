#Probabilità_e_statistica 
> [!definizione]  Definizione
> La [[Funzioni|funzione]] generatrice di momenti (MGF) è una funzione utilissima in probabilità e statistica, che ci permette di ottenere:
> - Il [[Valore Atteso]]
> - La [[Varianza]]
> - La Simmetria
> - La Curtosi
> 
> Essa è definita tale che:
> $$M_{X}(t)=\mathbb{E}[e^{tX}]\quad \quad \forall t\in\mathbb{R}$$

### <font color="#4bacc6">Come usare la MGF</font>:

Per poter ottenere i valori sopra indicati, dovremo fare una espansione di Taylor in $t=0$ della funzione, dopo una serie di vari passaggi matematici arriveremo a:
$$M_{X}(t)=\mathbb{E}[e^{tX}]=\sum_{k=0}^\infty\mathbb{E}[X^k] \frac{t^k}{k!}$$

Il primo momento ($k=1$) ci dice il Valore Atteso
Il secondo momento ($k=2$) ci dice la Varianza

Per poter calcolare la varianza allora faremmo:
$$M_{X}'(0)=\mathbb{E}(X)$$
$$M_{X}''(0)=\mathbb{E}(X^2)$$
Allora:
> [!dimostrazione] Dimostrazione
> Abbiamo la $Var(X)=\mathbb{E}[(X-\mathbb{E}[X])^2]$