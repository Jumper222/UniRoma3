---
tags:
  - Probabilità_e_statistica
aliases:
  - Processo di Bernoulli
  - Processo di Poisson
---
>[!Definizione]  Definizione
>Il Processo di Bernoulli studia una sequenza di [[Eventi]] indipendenti che possono avere il risultato binario di successo o insuccesso.


Allora abbiamo che la possibilità di successo è descritta da $p$, e quella di insuccesso da $1-p$.
Formalizzando:

Abbiamo una successione [[IID]] di [[Variabili Aleatorie di Bernoulli|v.a. Bernoulliane]], con $Bern(p)$, rappresentiamo queste v.a. con $B_{i}$ dove $i$ è il numero della variabile nella successione.

Allora vogliamo contare il numero di successi in un dato intervallo:

In un dato intervallo $[s+1,\dots,t]$ il numero di successi è dato dalla sommatoria:
$$\sum^t_{i=s+1}B_{i}$$
Questa sommatoria è anche 
