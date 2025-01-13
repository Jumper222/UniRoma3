---
tags:
  - geometria_e_combinatoria
---
La Molteplicità di un autovettore sta a significare la “potenza” della radice del polinomio semplificato.

> [!definizione]
> Sia $a$ una radice del polinomio $p(x)$.
> Allora $a$ è radice di $p(x)$ con molteplicità $m$ se $p(x)=(x-a)^m\ k(x)$ con $k(a)\neq0$.
> Ossia, $a$ ha molteplicità $m$ se:
> $(x-a)^m$ divide $p(x)$, mentre $(x-a)^{m+1}$ non lo divide.

Ad esempio:
$$p(x):=2x^5+2x^4-4x^3-2x^2-2x+4$$
Scopriamo che il polinomio è divisibile per 1, ossia da resto 0 se sostituiamo ad $x$ il numero 1:
$$p(1)=0\to p(x)=(x-1)(2x^4+4x^3-2x-4)$$
Però possiamo anche notare che $1$ è ancora divisione:
$$p(1)=0\to p(x)=(x-1)^2(2x^3+6x^2+6x+4)$$
Abbiamo quindi la <font color="#f79646">radice</font> $1$ di <font color="#9bbb59">grado</font> $2$.


