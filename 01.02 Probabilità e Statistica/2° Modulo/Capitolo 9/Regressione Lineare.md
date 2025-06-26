Date delle coppie di dati $((x_{1},y_{1}),\dots,(x_{n},y_{n}))$, voglio predire $y_{n+1}$ conoscendo solo $x_{n+1}$

Poniamo allora $Y$ come variabile dipendente, e risolviamo l’ equazione:

$$Y=\alpha+\beta x+Z$$
- Con $\alpha,\beta,\sigma^2$ parametri 
- $x$ come valore in input (Variabile indipendente, nota)
- $Z$ come errore $\mathcal{N}(0,\sigma^2)$
- Avendo gli errori con una media $=0$, allora il $\mathbb{E}[Y]=\alpha+\beta x$

Allora possiamo dire che $Y\sim\mathcal{N}(\alpha+\beta x,\sigma^2)$

Vogliamo quindi stimare sulla base dei dati raccolti $\alpha,\beta,\sigma^2$

Chiamo allora $A$ lo stimatore per $\alpha$, e $B$ lo stimatore per $\beta$

Ora considero la somma degli scarti quadratrici: 

$$SS=\sum^n_{i=1}(Y_{i}-(A+Bx_{i}))^2$$
Ora per trovare $A,B$ deriviamo rispetto ad $A,B$ questa formula e la poniamo $=0$ in un sistema:

$$\dfrac{\delta SS}{\delta A}=-2\sum^n_{i=1}(Y_{i}-(A+Bx_{i}))^2$$
$$\dfrac{\delta SS}{\delta B}=-2\sum^n_{i=1}x_{i}(Y_{i}-A-Bx_{i})$$
Quindi pongo a sistema:
$$\begin{cases}
\dfrac{\delta SS}{\delta A}=0 \\
\dfrac{\delta SS}{\delta B}=0
\end{cases}$$

Risolvendo il sistema otterremo una soluzione del tipo:
$$\begin{cases}
A=\bar{Y}-B\bar{x} \\
B=\dfrac{\sum^n_{i=1}Y_{i}(x_{i}-\bar{x})}{\left( \sum^n_{i=1} \right)-n\bar{x}^2}
\end{cases}$$

Per questa scelta di $A$,$B$ chiamerò $y=A+Bx$ la <font color="#f79646">retta di regressione stimata</font>