#Geometria_e_Combinatoria 
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
$$dim\ E(0)=4-rk(A-0I)=4-rk\begin{pmatrix}
2 & 1 & 0 & 0 \\
0 & 2 & 1 & 0 \\
0 & 3 & 0 & 2 \\
2 & 6 & 1 & 2
\end{pmatrix}=4-3=1$$

<font color="#f79646">MA</font> $1\neq 2$, ossia la molteplicità di $0$. quindi abbiamo che $f$ non è diagonalizzabile.

### <font color="#4bacc6">Esempio 3</font>
Sia dato l’ endomorfismo $f:M(2,2,R)\to M(2,2,R)$:
$$f\begin{pmatrix}
a & b \\
c & d
\end{pmatrix} := \begin{pmatrix}
a + 2b + d & a + d \\
a + b + d & a + b + d
\end{pmatrix}$$
La mat. rappresentativa rispetto la base canonica è:
$$A := \begin{pmatrix}
1 & 2 & 0 & 1 \\
1 & 0 & 0 & 1 \\
1 & 1 & 0 & 1 \\
1 & 1 & 0 & 1
\end{pmatrix}$$
Avremo quindi il polinomio caratteristico: 
$$p_f(x) = \begin{vmatrix}
1-x & 2 & 0 & 1 \\
1 & -x & 0 & 1 \\
1 & 1 & -x & 1 \\
1 & 1 & 0 & 1-x
\end{vmatrix}$$
Esplicitiamolo:
$$p_{f}(x)=x^4-2x^3-3x^2=x^2(x^2-2x-3)$$

Quindi trovate le radici, esse saranno $-1,+3$, entrambe di molteplicità = 1.

Avremo quindi una semplificazione in:
$$p_{f}(x)=x^2(x-3)(x+1)$$
Quindi la prima condizione è soddisfatta, ora vediamo la seconda, per la radice 0 di molteplicità 2.

$$dim\ E(0)=4-rk(A-0I)=2$$
<font color="#f79646">ALLORA</font> abbiamo che $f$ è diagonalizzabile!
<font color="#ffff00">Ossia</font> $f$ è rappresentabile con una matrice diagonale rispetto ad una base.

E quindi diagonalizziamola!

Abbiamo quindi l’ endomorfismo $f$ che è rappresentabile con la matrice diagonale $D$ rispetto ad una base.

$$D:= \begin{pmatrix}
0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 \\
0 & 0 & -1 & 0 \\
0 & 0 & 0 & 3
\end{pmatrix}$$
- Ogni autovalore è riportato lungo la diagonale un numero di volte uguale alla sua molteplicità.

Calcoliamo la base rispetto a cui $f$ si rappresenta con la matrice $D$, per farlo dovremo trovare una base per ciascun autospazio ed unirle. Questa base dovrà essere formata da autovettori di $f$.


Iniziamo allora con l’ autospazio di $0$:

Quello che faremo sarà moltiplicare l’ autospazio di $0$ (Ossia $A-0I$) per un vettore generico ($x,y,z,w$) e li porremo uguali a 0. risolveremo tutto quindi con un sistema.

Matrice dell’ autospazio d 0:

$$A := \begin{pmatrix}
1 & 2 & 0 & 1 \\
1 & 0 & 0 & 1 \\
1 & 1 & 0 & 1 \\
1 & 1 & 0 & 1
\end{pmatrix}$$
Creazione del sistema:

$$ \begin{pmatrix}
1 & 2 & 0 & 1 \\
1 & 0 & 0 & 1 \\
1 & 1 & 0 & 1 \\
1 & 1 & 0 & 1
\end{pmatrix}*\begin{pmatrix}
x \\
y \\
z \\
w
\end{pmatrix}=\begin{pmatrix}
0 \\
0 \\
0 \\
0
\end{pmatrix}\to \begin{cases}
x+2y+w&=0 \\
x\phantom{2222.}+w&=0 \\
x+\phantom{2}y+w&=0 \\
x+\phantom{2}y+w&=0

\end{cases}$$
Notiamo che in questo sistema ci sono 2 equazioni linearmente dipendenti, ossia la 3° e 4° riga. Allora possiamo decidere di parametrizzare 2 variabili, in questo caso avremo $z=t$ e $w=u$, da cui deriverà che $x=-u$, ed infine avremo $y=0$

Allora il risultato del sistema sarà:
$$\begin{cases}
x=-u \\
y=0 \\
z=t \\
w=u
\end{cases}$$

Avremo allora che $E(0)=\{-uE_{{11}}+tE_{21}+uE_{22}\}$ e allora la base di $E(0)$ sarà $-E_{{11}}+E_{{22}};E_{21}$

Ora facciamo un procedimento analogo per $E(-1)$:
$$\begin{pmatrix}
2 & 2 & 0 & 1 \\
1 & 1 & 0 & 1 \\
1 & 1 & 1 & 1 \\
1 & 1 & 0 & -2
\end{pmatrix}*\begin{pmatrix}
x \\
y \\
z \\
w
\end{pmatrix}=\begin{pmatrix}
0 \\
0 \\
0 \\
0
\end{pmatrix}\to \begin{cases}
2x+2y\phantom{+2z}+\phantom{2}w&=0 \\
\phantom{2}x+\phantom{2}y\phantom{+2z}+\phantom{2}w&=0 \\
\phantom{2}x+\phantom{2}y+z+\phantom{2}w&=0 \\
\phantom{2}x+\phantom{2}y\phantom{+2z}+2w&=0
\end{cases}$$

Il sistema darà come risultato
$$\begin{cases}
x=-t \\
y=t \\
z=0 \\
w=0
\end{cases}$$
Quindi avremo che $E(-1)=\{-tE_{11}+tE_{12}\}$ formano la base: $-E_{11}+E_{12}$

Facciamo lo stesso con $E(3)$ e avremo come risultato:
$$\begin{cases}
x=\frac{5}{4}t \\
y=\frac{3}{4}t \\
z=t \\
w=t
\end{cases}$$
E quindi la base di $E(3)$ sarà: $\frac{5}{4}E_{11}+\frac{3}{4}E_{12}+E_{21}+E_{22}$

Quindi traduciamo tutto con le basi dell’ omomorfismo, moltiplicando i prodotti scalari delle basi con le basi stesse.

Base per $E(0)$:
$$A_{1}:=\begin{pmatrix}
-1 & 0 \\
0 & 1
\end{pmatrix};A_{2}:=\begin{pmatrix}
0 & 0 \\
1 & 0
\end{pmatrix}$$
Base per $E(-1)$:
$$A_{3}:=\begin{pmatrix}
-1 & 1 \\
0 & 0
\end{pmatrix}$$
Base per $E(3)$:
$$A_{4}:=\begin{pmatrix}
\frac{5}{4} & \frac{3}{4} \\
1 & 1
\end{pmatrix}$$

Quindi creiamo la matrice di passaggio dalla base canonica a questa base:
$$M:=\begin{pmatrix}
-1 & 0 & -1 & \frac{5}{4} \\
0 & 0 & 1 & \frac{3}{4} \\
0 & 1 & 0 & 1 \\
1 & 0 & 0 & 1
\end{pmatrix}$$
L’ esercizio è finito.