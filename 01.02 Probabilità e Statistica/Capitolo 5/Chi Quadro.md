#Probabilità_e_statistica 

>[!Definizione]  Definizione
>Il Chi-Quadrato (o quadro), indicato con $\mathcal{X}$ è una famiglia di distribuzioni di probabilità [[Variabili Aleatorie discrete e continue|continua]] che dipende da un parametro di libertà $k$.
>Queste distribuzioni si ottengono sommando tra loro i quadrati di k [[Gaussiana Standard|Gaussiane standard]], ossia [[Variabili Aleatorie Gaussiane|v.a. Gaussiane]] con [[Valore Atteso]] = 0 e [[Varianza]] = 1.
>Allora Chi-Quadro è definito tale che:
>$$\mathcal{X}^2=Z^2_{1}+Z^2_{2}+\dots+Z^2_{k}$$
>Allora avremo che il [[Valore Atteso]]:
>$$\mathbb{E}[X]=k$$
>E la [[Varianza]]:
>$$Var(X)=2k$$
### <font color="#4bacc6">Proprietà di Chi Quadro</font>

Esattamente come le [[Variabili Aleatorie Gaussiane|v.a. Gaussiane]], anche Chi Quadro è riproducibile, ossia:

Se $X\sim\mathcal{X}^2_{n}$ e $Y\sim\mathcal{X}^2_{m}$, indipendenti, allora
$$X+Y\sim \mathcal{X}^2_{n+m}$$
Un’ altra utile proprietà è che la distribuzione Chi Quadro è simmetrica e positiva, e man mano che  aumentano i gradi di libertà la distribuzione si avvicina sempre più ad una [[Gaussiana Standard]]

Esattamente come per le [[Variabili Aleatorie Gaussiane|v.a. Gaussiane]], anche per Chi Quadro possiamo studiare il [[Punto Critico Chi Quadro]]


### <font color="#4bacc6">PDF di Chi Quadro</font>

![[PDF Chi Quadro.png]]