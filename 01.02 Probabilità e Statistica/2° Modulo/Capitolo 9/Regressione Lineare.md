Date delle coppie di dati $((x_{1},y_{1}),\dots,(x_{n},y_{n}))$, voglio predire $y_{n+1}$ conoscendo solo $x_{n+1}$

Poniamo allora $Y$ come variabile dipendente, e risolviamo l’ equazione:

$$Y=\alpha+\beta x+Z$$
- Con $\alpha,\beta,\sigma^2$ parametri 
- $x$ come valore in input (Variabile indipendente, nota)
- $Z$ come errore $\mathcal{N}(0,\sigma^2)$

Allora possiamo dire che $Y\sim\mathcal{N}(\alpha+\beta x,\sigma^2)$

Vogliamo quindi stimare sulla base dei dati raccolti $\alpha,\beta,\sigma^2$

Chiamo allora $A$ lo stimatore per $\alpha$, e $B$ lo stimatore per $\beta$

Ora considero la somma degli scarti quadratrici: 

$$SS=\sum^n$$