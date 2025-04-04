#Geometria_e_Combinatoria 
Dati 2 [[Sottospazi vettoriali]] $E$ ed $F$ di uno spazio vettoriale $V$, vedremo che:

- L’ intersezione di $E$ ed $F$ ($E\cap F$) è un sottospazio vettoriale
- L’ unione di $E$ ed $F$ <font color="#f79646">non</font> è sempre un sottospazio vettoriale.

### Intersezione 

$E\cap F$ è sempre un sottospazio vettoriale sia di $E$ che di $F$. 
$dim\ (E\cap F)\leq dim\ E$
$dim\ (E\cap F)\leq dim\ F$

---

Qualche esempio sulle intersezioni:

Siano dati i seguenti sottospazi $E$, $F$ di $M(2,2,R)$:
$$E:=\begin{pmatrix}
a & b \\
b & 0
\end{pmatrix};\ F:=\begin{pmatrix}
b & a \\
b & 0
\end{pmatrix}$$
Allora diamo una generica matrice $A$, definita da 4 valori generici:
$$A:=\begin{pmatrix}
a_{11} & a_{12} \\
a_{21} & a_{22}
\end{pmatrix}$$
Potremo quindi dire che $A$ appartiene ad $E$ solo se $a_{22}=0$ e $a_{12}=a_{21}$
E anche che $A$ appartiene ad $E$ solo se $a_{22}=0$ e $a_{11}=a_{21}$

Allora:
$$E\cap F=\begin{pmatrix}
a & a \\
a & 0
\end{pmatrix}$$
Questo esercizio è piuttosto banale, vediamone uno più difficile:

----

Determinare $E\cap F$, considerando in $R^5$:

$E$ generato da $e_{1}:=(1,4,0,0,0),\ e_{2}:=(1,0,0,1,1),\ e_{3}:=(1,1,0,-1,2)$
$F$ generato da $f_{1}:=(2,1,1,4,0),\ f_{2}:=(-1,1,-1,0,2)$

Allora avremo un generico vettore $v_{1}$:
$$v_{1}=h_{1}(1,4,0,0,0)+h_{2}(1,0,0,1,1)+h_{3}(1,1,0,-1,2)$$
che si traduce in:
$$(h_{1}+h_{2}+h_{3},4h_{1}+h_{3},0,h_{2}-h_{3},h_{2}+2h_{3})$$
Ed un secondo vettore generico $v_{2}$:
$$v_{2}=k_{1}(2,1,1,4,0)+k_{2}(-1,1,-1,0,2)$$
che si traduce in:
$$(2k_{1}-k_{2},k_{1}+k_{2},k_{1}-k_{2},4k_{1},2k_{2})$$


