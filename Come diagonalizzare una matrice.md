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

### <font color="#4bacc6">Esempio 1</font>
Sia data la matrice $A$ ed il suo polinomio caratteristico:
$$A := \begin{pmatrix}
2 & 1 & 0 & 0 \\
0 & 2 & 1 & 0 \\
0 & 0 & 0 & 2 \\
-4 & 0 & 1 & 2
\end{pmatrix}
\begin{vmatrix}
2-x & 1 & 0 & 0 \\
0 & 2-x & 1 & 0 \\
0 & 0 & 0-x & 2 \\
-4 & 0 & 1 & 2-x
\end{vmatrix}$$
$$p_{A}(x):=\det(A-xI)=x^4-6x^3+10x^2=x^2(x^2-6x+10)$$
Quindi proviamo a semplificare ancora, calcolando $\Delta$, purtroppo esso è minore di zero, quindi non ci sono radici reali.

<font color="#f79646">Allora</font> il polinomio caratteristico di $A$ non è totalmente riducibile,
<font color="#f79646">Allora</font> la matrice $A$ non è diagonalizzabile.

### <font color="#4bacc6">Esempio 2</font>
Consideriamo l’ endomorfismo di $R^4$ definito da:
$$f(x,y,z,w):=(2x+y,2y+z,3y+2w,2x+6y+z+2w)$$
La matrice rappresentativa rispetto la base canonica sarà:
$$A := \begin{pmatrix}
2 & 1 & 0 & 0 \\
0 & 2 & 1 & 0 \\
0 & 3 & 0 & 2 \\
2 & 6 & 1 & 2
\end{pmatrix}
\qquad
p_A(x) := \begin{vmatrix}
2-x & 1 & 0 & 0 \\
0 & 2-x & 1 & 0 \\
0 & 3 & 0-x & 2 \\
2 & 6 & 1 & 2-x
\end{vmatrix}$$
Il suo polinomio caratteristico sarà:
$$p_{f}(x):=x^4-6x^3+7x^2=x^2(x^2-6x+7)$$
Calcoliamo la scomposizione del polinomio di secondo grado con la formula della parabola:
$$x_{1},x_{2}=\frac{6\pm \sqrt{8}}{2}=3\pm \sqrt{ 2 }$$
<font color="#f79646">Allora</font> il polinomio caratteristico è <font color="#ffff00">totalmente riducibile</font>, infatti ha gli autovalori:
- $0$ di molteplicità $2$
- $3+\sqrt{ 2 }$ di molteplicità $1$
- $3-\sqrt{ 2 }$ di molteplicità $1$
quindi la prima condizione è rispettata.

Iniziamo quindi a calcolare se la molteplicità dei valori coincide con la dimensione del relativo autospazio.

Iniziamo con $0$:


