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