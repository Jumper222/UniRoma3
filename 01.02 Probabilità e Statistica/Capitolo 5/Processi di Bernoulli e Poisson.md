---
tags:
  - Probabilità_e_statistica
aliases:
  - Processo di Bernoulli
  - Processo di Poisson
---
### <font color="#4bacc6">Processo di Bernoulli</font>

>[!Definizione]  Definizione
>Il Processo di Bernoulli studia una sequenza di [[Eventi]] indipendenti che possono avere il risultato binario di successo o insuccesso.


Allora abbiamo che la possibilità di successo è descritta da $p$, e quella di insuccesso da $1-p$.
Formalizzando:

Abbiamo una successione [[IID]] di [[Variabili Aleatorie di Bernoulli|v.a. Bernoulliane]], con $Bern(p)$, rappresentiamo queste v.a. con $B_{i}$ dove $i$ è il numero della variabile nella successione.

Allora vogliamo contare il numero di successi in un dato intervallo:

In un dato intervallo $[s+1,\dots,t]$ il numero di successi è dato dalla sommatoria: (stiamo aggiungendo 1 ad s in modo da non contare la prova s, per scelta nostra.)
$$\sum^t_{i=s+1}B_{i}$$
Questa sommatoria è distribuita come una [[Variabili Aleatorie Binomiali|v.a. Binomiale]]:
$$\sim Bin(t-s,p)$$
E se invece volessimo sapere quando sarà il prossimo successo useremmo una [[Variabili Aleatorie Geometriche|v.a. Geometrica]]:
$$\sim Geom(p)$$

Questo processo ha senso per le [[Variabili Aleatorie discrete e continue|v.a. discrete]], per quelle [[Variabili Aleatorie discrete e continue|v.a. continue]] invece usiamo il <font color="#ffff00">Processo di Poisson</font>

### <font color="#4bacc6">Processo di Poisson</font>

>[!Definizione]  Definizione
>Il Processo di Poisson è un modello che serve per studiare la probabilità che si verifichino un numero di eventi in un dato tempo, ha dei requisiti:
>- Un rateo $\lambda$, 
Ricordandoci sempre che andiamo a studiare un’ intervallo $[s,t]$, dove entrambi sono maggiori di 0, dove $k$ è il valore che stiamo cercando la probabilità degli eventi sarà del tipo:
$$P(N(t)-N(s)=k)=e^{-\lambda(t-s)} \dfrac{(\lambda(t-s))^k}{k!}$$

Una proprietà dei processi di Poisson è che prendendo intervalli diversi essi sono indipendenti tra loro:
$$\forall t_{2}>s_{2}>t_{1}>s_{1}\geq 0$$
$N(t_{2})-N(s_{2})$ è indipendente da $N(t_{1})-N(s_{1})$ 

*NB: in tutti questi esempi $N$ è una funzione che conta quante volte abbiamo un successo in un dato intervallo*

Allora un Processo di Poisson avrà una forma del tipo:

![[Processo di Poisson.png]]

### <font color="#4bacc6">Tempi di Arrivo</font>


I tempi di arrivo (quando abbiamo un successo) li chiameremo $T_{1},T_{2}\dots$ e quelli di inter-arrivo saranno definiti da
$$X_{k}=T_{k}-T_{k-1}$$
Per convenzione diamo che $T_{0}=0$

Per quanto riguarda la distribuzione dei tempi di inter-arrivo, essi sono distribuiti come
$$e^{-\lambda t}$$
Proprio qui entrano in gioco le [[Variabili Aleatorie Esponenziali|v.a. esponenziali]], infatti la successione dei tempi di inter-arrivo $X_{1},X_{2}\dots$ è una successione di [[Variabili Aleatorie|v.a.]] [[IID]] $Exp(\lambda)$ 

Un’ altra particolarità è che se sappiamo che fino al tempo $t$ c’è un unico successo, allora $T_{1}$ sarà distribuito come $\dfrac{s}{t}$, dove s è il lower bound dell’ intervallo che stiamo considerando. Questa distribuzione è la stessa di una [[Variabili Aleatorie Uniformi|v.a. Uniforme]] 

>[!Osservazione]  Osservazione
>Per svolgere gli esercizi è utile ricordarsi che se prendiamo $n$ [[Variabili Aleatorie Uniformi|v.a. uniformi]] $U_{1},U_{2},\dots,U_{n}$ [[IID]] e chiamiamo $U_{k}$ la k-esima variabile più piccola; “k-esima statistica ordinata”
>Allora abbiamo che
>$$(T_{1},\dots,T_{n})|N(t)=n\sim(tU_{(1)},\dots,tU_{(n)})$$
>Quindi, se voglio campionare un processo di Poisson di tasso $\lambda$ in un intervallo $[0,t]$ posso procedere come segue:
>1. campiono $N(t)\sim Poi(\lambda t)$ (Chiamo $n$ il numero ottenuto)
>2. campiono $U_{1},\dots,U_{n}$ [[IID]] $Unif[0,1]$ e chiamo $u_{1},\dots,u_{n}$ il numeri ottenuti una volta ordinati dal più piccolo al più grande
>3. Pongo $T_{1}=tu_{(1)},\dots,T_{n}=tu_{(n)}$

