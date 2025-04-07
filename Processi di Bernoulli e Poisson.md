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
>Il processo di Poisson $(N(t))_{t\geq 0}$ è detto Processo di Poisson di intensità/tasso $\lambda>0$ è la [[Funzioni|funzione]] aleatoria a valori $\geq 0$ t.c:
>Il maggiore utilizzo del processo di Poisson si ha trovando i tempi di arrivo, ossia quando si ha un successo in una funzi

