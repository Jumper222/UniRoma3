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

Per quanto riguarda la varianza degli stimatori:

$$Var(A)=\sigma^2 \dfrac{\dfrac{1}{n}\sum^n_{i=1}x^2_{i}}{\sum^n_{i=1}x^2_{i}-n\bar{x}^2}$$
$$Var(B)=\sigma^2 \dfrac{1}{\sum^n_{i=1}x^2_{i}-n\bar{x}^2}$$

Però qui mi viene chiesto di stimare $\sigma^2$, e per farlo dovrò stimare i “Residui”, ossia l’ errore dato all’ approssimare $Y_{i}$ con $A+Bx_{i}$, Questi residui avranno quindi la forma:
$$Y_{i}-(A+Bx_{i})$$

Chiamo allora $SS_{R}$ la somma dei quadrati dei residui:
$$SS_{R}=\sum^n_{i=1}[Y_{i}-(A+Bx_{i})]^2$$
Può essere dimostrato che $\dfrac{1}{\sigma^2}SS_{R}\sim \chi^2_{n-2}$
E per definizione di [[Chi Quadro]], il suo valore atteso è uguale ai suoi gradi di libertà, quindi:
$$\sigma^2=\dfrac{\mathbb{E}[SS_{R}]}{n-2}$$
E allora uno stimatore non distorto di $\sigma^2$ è dato da:
$$\dfrac{SS_{R}}{n-2}$$

Avendo molte somme, è utile la seguente notazione:

$$S_{XY}=\sum^n_{i=1}(x_{i}-\bar{x})(Y_{i}-\bar{Y})$$
$$S_{XX}=\sum^n_{i=1}(x_{i}-\bar{x})^2$$
$$S_{YY}=\sum^n_{i=1}(Y_{i}-\bar{Y})^2$$
E allora definiamo $SS_{R}$ in funzione di queste notazioni:
$$SS_{R}=\dfrac{S_{XX}S_{YY}-S^2_{XY}}{S_{XX}}$$

Riassumendo:

- $B=\dfrac{S_{XY}}{S_{XX}}\sim\mathcal{N}(\beta, \dfrac{\sigma^2}{S_{XX}})$
- $A=\bar{Y}-B$