---
tags:
  - Probabilità_e_statistica
aliases:
  - v.a. Geometriche
  - v.a. geometriche
---

>[!Definizione]  Definizione
>Le [[Variabili Aleatorie|v.a.]] geometriche ci servono per sapere quanti tentativi servono in media per ottenere il primo successo in una serie di esperimenti casuali indipendenti tra loro, ed è descritta:
>Nelle [[Variabili Aleatorie|v.a.]] Geometriche $X$ rappresenta il tempo in cui arriva il primo successo in una successione di esperimenti [[IID]] in cui ciascun esperimento ha successo = p.
>$$X\sim Geom(p)$$
>E la sua PMF è definita t.c:
>$$P(Y=y)=f_{X}=p(1-p)^{y-1}$$
>Il suo [[Valore Atteso]] invece sarà nella forma:
>$$\mathbb{E}[X]=\dfrac{1}{p}$$
>E la sua [[Varianza]]:
>$$Var(X)=\dfrac{1-p}{p^2}$$
>Formula utile per maggiori o minori di numero x, in caso di minore si usa il complementare
> $$Y \sim \text{Geom}(p) \implies \mathbb{P}(Y>y) = (1-p)^y \quad \forall y \geq 1$$

Una molto particolare proprietà delle [[Variabili Aleatorie|v.a.]] geometriche è detta Assenza di Memoria o Memorylessness,
è significa che gli esiti degli eventi precedenti a quello attuale non impattano per nulla la probabilità dell’ evento studiato.

La PMF appare nella forma:
![[PMF v.a. Geom.png]]