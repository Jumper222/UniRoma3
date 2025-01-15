---
tags: geometria_e_combinatoria
---
Il nostro primo obiettivo è trovare un <font color="#ffff00">criterio</font> per stabilire se un dato endomorfismo possa essere diagonalizzabile o no.

Se troviamo che sia diagonalizzabile allora descriviamo il procedimento per farlo.

---

Facciamo un esempio, così da avere il criterio ed il procedimento in atto.

Sia $f:R^4[x]\to R^4[x]$ l’ endomorfismo che associa al polinomio $a_{0}+a_{1}x+a_{2}x^2+a_{3}x^3$ al polinomio 
$$(a_{0}+a_{1})+(a_{1}-a_{2}+a_{3})x+(a_{0}+2a_{1}-a_{2})x^2+3a_{3}x^3$$
Consideriamo quindi la base canonica di $R^4$ per la matrice rappresentativa.

<font color="#ffff00">Allora</font> calcoliamo le radici del pol. caratteristico $p_{f}(x):=\det(A-xI)$
Troviamo allora gli autovalori $0$ ed $1$.

Entrambi gli autospazi hanno $dim=1$.

<font color="#4bacc6">Quindi</font> ci possiamo chiedere se $f$ è diagonalizzabile,
Ovvero se esiste una base per $R^4[x]$ formata dagli autovettori di $f$.

Dato che $dim\ E(0)=1$ e $dim\ E(1)=1$, è impossibile che tutti e 4 i polinomi
che formano la base canonica di $R^4$ possano diventare autovettori.

<font color="#f79646">Allora</font> $f$ non è diagonalizzabile.

---

enunciamo quindi qualche teorema legato alla diagonalizzazione:

> [!Enunciato]
> Sia $f:V\to V$ un’ endomorfismo di uno spazio vett. $V$ di dim. finita $n$ e siano $1,2,\dots,s$ gli autovalori distinti di $f$. 
> Se $dim\ E(1)+dim\ E(2)+\dots+dim\ E(s)<n$ allora $f$ <font color="#c0504d">non</font> è diagonalizzabile.
> In altre parole, affinchè $f$ sia diagonalizzabile è necessario che
> $dim\ E(1)+dim\ E(2)+\dots+dim\ E(s)=n$

> [!enunciato]
    > Sia $f:V\to V$ un endomorfismo di uno spazio vett. $V$ di dim finita $n$ e siano $1,2,\dots,s$ gli autovalori distinti di $f$.
    > Prendiamo una base per ciascun autospazio: unendo tali basi si ottengono dei vettori tra loro <font color="#ffff00">linearmente indipendenti</font>.
    > Dunque, abbiamo dei autovettori <font color="#ffff00">linearmente indipendenti</font>.
    > In particolare: $dim\ E(1)+dim\ E(2)+\dots+dim\ E(s)\leq n$

> [!osservazione]
> Sappiamo che per ciascun autovalore $i$ si ha $dim\ E(i)\leq m_{f}(i)$
> Ossia:
> $$dim\ E(1)+dim\ E(2)+\dots+dim\ E(s)\leq m_{f}(1)+m_{f}(2)+\dots+m_{f}(s)\leq n$$
> Allora possiamo riassumere tutto con:
> Affinché $f$ sia diagonalizzabile è necessario che la somma delle molteplicità degli autovalori sia uguale ad $n$, ovvero il <font color="#ffff00">polinomio caratteristico</font> di $f$ deve essere <font color="#f79646">totalmente riducibile</font>.
>      
>  Se anche per uno solo degli autovettori $i$ si ha: $dim\ E(i)<m_{f}(i)$
>  <font color="#f79646">allora</font> $f$ non è diagonalizzabile.
> 

> [!enunciato]
    > Se $f$ è un’ endomorfismo, esso sarà diagonalizzabile se e solo se:
    > 1. Il polinomio caratteristico di $f$ è totalmente riducibile.
    > 2. per ciascun autovalore $i$ di $f$ si ha $dim\ E(i)=m_{f}(i)$.
    > > [!osservazione]
    > > Se $\lambda$ è un autovalore semplice allora $dim\ E(\lambda)=1$
    > > La seconda condizione del teorema va quindi verificata solo per gli autovalori di molteplicità almeno 2.  

### La base particolare

Per calcolare una base di $V$ formata dagli autovettori di $f$ si prende una base per ciascun autospazio e le si uniscono.
Rispetto a tale base $f$ si presenta come una matrice diagonale, i cui elementi lungo la diagonale sono gli autovalori di $f$, ciascuno ripetuto un numero di volte pari alla sua molteplicità.

---


### Metodo per individuare se un endomorfismo è diagonalizzabile

> [!osservazione]
> Sia $f:V\to V$ un endomorfismo di uno spazio vettoriale $v$ di dim. finita $n$.
> 1. Scegliere $e_{1},e_{2},\dots,e_{n}$ vettori che formano una base di $V$.
> 2. Calcolare la matrice $A$ rappresentativa di $f$ rispetto la base scelta.
> 3. Definire il polinomio (di grado $n$) caratteristico di $f:p_{f}(x):=\det(A-xI)$
> 4. Risolvere $\det(A-xI)=0$. Le soluzioni sono gli autovalori di $f$.
>     Se $f$ non è totalmente riducibile, $f$ non è diagonalizzabile. <font color="#f79646">STOP</font>
> 5. Per ciascun autovalore (di molteplicità $>1$) verificare se la sua molteplicità e la dim. del suo autospazio coincidono.
> 6. Se esiste almeno un valore $\lambda_{i}$ per cui si ha $dim\ E(\lambda_{i})<m(\lambda_{i})$
>     allora $f$ non è diagonalizzabile, <font color="#f79646">STOP</font>
> 7. Se per tutti gli autovalori $\lambda_{i}$ si ha $dim\ E(\lambda_{i})=\lambda_{i}$
>     allora $f$ è diagonalizzabile, <font color="#f79646">STOP</font>
>     


[[Esempi sulla diagonalizzazione]]