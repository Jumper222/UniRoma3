---
tags:
  - Probabilità_e_statistica
aliases:
  - CDF
---

>[!Definizione]  Definizione
>La [[Funzioni|Funzione]] di ripartizione (Anche chiamata Cumulative Distribution Function) (CDF in <font color="#8db3e2">inglese</font>) di $X$ è la funzione che ci dice quanto è probabile che la variabile aleatoria assuma un valore minore o uguale ad un dato numero
>Ed è definita:
>$$F_{X}​(x)=P(X≤x)$$
>Alcune utili info:
>- Cresce sempre da 0 ad 1
>- La funzione di Ripartizione ti dice la probabilità che $X$ sia al massimo $x$
>- La funzione è sempre non-decrescente, ossia man mano che $x$ cresce, la probabilità non può diminuire

Esempio:

Abbiamo $X$ che è il risultato del lancio di un dado

![[Lancio del dado Funzione di Ripartizione.png]]

La potenza di un grafico di questo tipo è immensa, qualsiasi domanda sensata che ci potremmo porre riguardante una variabile aleatoria troverà la sua risposta in questo grafico.

Allora da questo grafico posso ottenere:
- $\mathbb{P}(X\leq4)=F_{x}(4)$
- $\mathbb{P}(X>4)=\mathbb{P}(\{X\leq 4\}^c)=1-\mathbb{P}(X\leq 4)=1-F_{x}(4)$
- $\mathbb{P}(2<X\leq 5)=F_{x}(5)-F_{x}(2)$
