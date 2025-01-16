Dati 2 sottospazi vettoriali $E$ ed $F$ di uno spazio vettoriale $V$, vedremo che:

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

