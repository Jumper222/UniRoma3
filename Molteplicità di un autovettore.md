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

---

Qui è utile ricordare che un polinomio di grado $n$ può avere gradi delle radici al massimo $\leq n$.

Riprendendo in esame l’ esempio di prima cerchiamo i divisori, dividendo il termine noto con il termine noto in $x$ del grado più alto. in questo caso faremmo $4/2=2$, quindi i possibili divisori sono $1,-1,2,-2$.

Quindi notiamo che $p(x)$ si annulla di nuovo per $x=-2$, allora facciamo una<font color="#f79646"> divisione di polinomi</font> o <font color="#f79646">Ruffini</font>, a seconda della semplicità, e troviamo:
$$(x-1)^2(x+2)(2x^2+2x+2)$$
Arrivati a questo punto per trovare altre radici possiamo calcolare il $\Delta$, che però si rivelerà negativo:
$$4-16<0$$
Il che significa <font color="#f79646">niente radici reali</font>, il che implica che il polinomio è semplificato al massimo.

Completata la semplificazione possiamo dire che il polinomio $p(x)$ ha radice $1$ di molteplicità $2$ e la radice $-2$ di molteplicità $1$. La somma di queste molteplicità è $3$, che è inferiore al grado di $p(x)$.<font color="#ffff00"> TUTTO TORNA!</font>

---

Un polinomio $p(x)$ di grado $n$ si dice totalmente riducibile se si può scrivere come prodotto di polinomi di $1°$ grado.