#Probabilità_e_statistica 
>[!Definizione]  Definizione
>La Varianza è quel valore che misura la dispersione dei dati rispetto al [[Valore Atteso]], ossia quanto sono “sparsi”
>Ed è definita:
>con v.a. X, e $\mu=\mathbb{E}[X]$
>Allora la varianza sarà tale che:
>$$Var(X)=\mathbb{E}[X^2]-(\mathbb{E}[X])^2$$
>
>Intuitivamente possiamo quindi dire che la varianza di $X$ è la differenza tra il momento $2°$ di X ed il quadrato del suo valore atteso.
>
>La varianza a differenza del valore atteso non rispetta sempre la proprietà ( la rispetta solo se $Cov(X,Y)=0$)
>$$Var(X+Y)=Var(X)+Var(Y)$$
>Infatti la formula corretta sarebbe:
>$$Var(X+Y)=Var(X)+Var(Y)+2Cov(X,Y)$$

> [!links]  Links
> A sua volta la varianza si connette con la [[Covarianza]] 
> 
> Per quanto riguarda le v.a. indicatrici, esiste un particolare modo di calcolare la [[Varianza di una v.a. indicatrice]]
> 
> Dal concetto di Varianza deriva direttamente la [[Deviazione Standard]] 
> 
> Il concetto di Varianza inoltre si applica come il valore atteso anche a [[Calcolare la varianza di una funzione|le funzioni di v.a.]]


Facciamo un semplice esempio: 
Supponiamo di avere una v.a. $X$ con i seguenti valori:
$\mathbb{P}(X=1)=0.5$
$\mathbb{P}(X=3)=0.5$

Calcoliamo il Valore Atteso:
$$\mathbb{E}[X]=(1*0.5)+(3*0.5)=0.5+1.5=2$$
Ora calcoliamo $\mathbb{E}[X^2]$:
$$\mathbb{E}[X^2]=(1^2*0.5)+(3^2*0.5)=(1*0.5)+(9*0.5)=0.5+4.5=5$$
Ora otteniamo la varianza con la formula ad inizio pagina:
$$Var(X)=\mathbb{E}[X^2]-(\mathbb{E}[X])^2=5-(2)^2=5-4=1$$
<font color="#f79646">Varianza = 1</font>
