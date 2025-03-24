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
Allora arriveremo nella forma:
$$e^{tX}=1+tX+\dfrac{t^2X^2}{2!}+\dfrac{t^3X^3}{3!}+\dots+\dfrac{t^nX^n}{n!}$$


Il primo momento ($k=1$) ci dice il Valore Atteso
Il secondo momento ($k=2$) ci porta poi alla Varianza (Non è la varianza!)

Per poter calcolare la varianza allora faremmo:
Momento primo:
$$M_{X}'(0)=\mathbb{E}(X)$$
Momento secondo:
$$M_{X}''(0)=\mathbb{E}(X^2)$$
Allora:
> [!dimostrazione] Dimostrazione
> Abbiamo la $Var(X)=\mathbb{E}[(X-\mathbb{E}[X])^2]$
> Allora sviluppiamo il quadrato:
> $$Var(X)=\mathbb{E}[X^2-2X\mathbb{E}[X]+(\mathbb{E}[X])^2]$$
> Quindi sfruttiamo le proprietà dell’ aspettazione:
> $$Var(X)=E[X^2]−2E[X]⋅E[X]+(E[X])^2$$
> Spostiamo le variabili:
> $$−2E[X]⋅E[X]+(E[X])^2=−(E[X])^2$$
> E allora abbiamo la nostra formula ben conosciuta per la varianza:
> $$Var(X)=\mathbb{E}[X^2]-(\mathbb{E}[X])^2$$

La particolarità della MGF sta nel fatto che 