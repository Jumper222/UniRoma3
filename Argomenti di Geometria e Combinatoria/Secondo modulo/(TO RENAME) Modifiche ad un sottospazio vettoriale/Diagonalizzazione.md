#Geometria_e_Combinatoria 

<font color="#f79646">NB</font>: è necessario avere bene a mente il concetto di [[Autovalore ed Autovettore|autovalore ed autovettore]]

---

Un endomorfismo $f$ si dice <font color="#f79646">diagonalizzabile</font> se esiste almeno una base di $V$ rispetto a cui $f$ si rappresenta con una <font color="#f79646">matrice diagonale</font>.

---

Facciamo immediatamente un semplice esempio:

sia $f$ l’ <font color="#ffff00">endomorfismo</font> di $R^2[x]$ definito da:
$f(a+bx):=2b+(-a+3b)x$

Possiamo dire che rispetto la base canonica $p_{1}(x):=1,p_{2}(x):=x$ questo <font color="#ffff00">endomorfismo</font> si presenta con la matrice $A$:
$$A=\begin{pmatrix}
0 & 2 \\
-1 & 3
\end{pmatrix}$$
Come notiamo immediatamente questa matrice non è <font color="#f79646">diagonale</font>, ciò nonostante l’ endomorfismo è <font color="#f79646">diagonalizzabile</font>, infatti se consideriamo invece della base canonica la base composta da $p_{1}(x):=1+x,p_{2}(x):=2+x$ avremo questa scomposizione:

- $f(p_{1}(x))=2+2x=2p_{1}(x)+0p_{2}(x)$
- $f(p_{2}(x))=2+x=0p_{1}+1p_{2}(x)$

otterremo la seguente matrice, <font color="#ffff00">diagonale</font>:
$$A'=\begin{pmatrix}
2 & 0 \\
0 & 1
\end{pmatrix}$$
Questo perché $f(p_{1}(x)),f(p_{2}(x))$ sono multipli di $p_{1}(x),p_{2}(x)$.

---

Allora diamo 