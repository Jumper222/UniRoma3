Data una matrice  $A\ (n\times n)$, 
Il polinomio caratteristico $p(\lambda)$ è un polinomio di grado $n$ in $\lambda$, ossia con variabili $\lambda$.
Ed è definito come determinante della matrice $A-\lambda I$, ossia:
$$p(\lambda)=\det(A-\lambda I)$$

Serve quindi per trovare gli autovalori, risolvendo l’ equazione:
$$\det(A-x I)=0$$
---

Facciamo quindi un esempio:

Sia $f:R^4[x]\to R^4[x]$ l’ endomorfismo che associa al polinomio:
$$a_{0}+a_{1}x+a_{2}x^2+a_{3}x^3$$
il polinomio::
$$(a_{0}+a_{1})+(a_{1}-a_{2}+a_{3})x+(a_{0}+2a_{1}-a_{2})x^2+a_{3}x^3$$

Considerando quindi per la matrice rappresentativa la base canonica otterremo:

$$\begin{pmatrix}
1 & 1 & 0 & 0 \\
0 & 1 & -1 & 1\\
1 & 2 & -1 & 0 \\
0 & 0 & 0 & 1 \\
\end{pmatrix}$$
Vogliamo ora determinare polinomi non nulli (questo è il polinomio caratteristico):
$$p(x):=a_{0}+a_{1}x+a_{2}x^2+a_{3}x^3$$
Allora riprendiamo la formula iniziale. applicandola otterremo:
$$\begin{pmatrix}
1 & 1 & 0 & 0 \\
0 & 1 & -1 & 1 \\
1 & 2 & -1 & 0 \\
0 & 0 & 0 & 1
\end{pmatrix}
\begin{pmatrix}
a_{0} \\
a_{1} \\
a_{2} \\
a_{3}
\end{pmatrix}=\lambda \begin{pmatrix}
a_{0} \\
a_{1} \\
a_{2} \\
a_{3}
\end{pmatrix}$$
che possiamo esplicitare in un sistema:
$$\begin{cases}
a_0 + a_1 &= \lambda a_0 \\
\phantom{123+.}a_1 - a_2 + a_3 &= \lambda a_1 \\
a_0 + 2a_1 - a_2 &= \lambda a_2 \\
\phantom{a_0 + 2a_1+1+..} a_3 &= \lambda a_3
\end{cases}$$
Che quindi può essere riscritto:
$$\begin{cases}
(1-x)a_0 +\phantom{11333,} a_1 &= 0 \\
\phantom{8191933333}(1-x)a_1 -\phantom{33333,,} a_2 +\phantom{333,} a_3 &= 0 \\
\phantom{333333}a_0 +\phantom{33333} 2a_1 + (1-x)a_2 &= 0 \\
\phantom{1+1+1+1+1+133333333333}(1-x)a_3 &= 0
\end{cases}$$
Se allora volessimo riscrivere il sistema in forma matriciale:
$$\begin{pmatrix}
1-x & 1 & 0 & 0 \\
0 & 1-x & -1 & 1 \\
1 & 2 & -1-x & 0 \\
0 & 0 & 0 & 1-x
\end{pmatrix}
\begin{pmatrix}
a_0 \\
a_1 \\
a_2 \\
a_3
\end{pmatrix}
=
\begin{pmatrix}
0 \\
0 \\
0 \\
0
\end{pmatrix}$$
Allora il polinomio caratteristico sarà proprio:
$$p(x):=\det(A-xI)$$
Gli autovalori saranno le radici di questo polinomio, avremo quindi come risultato:
$$(1-x)(-x^3+x^2-x)$$
Che poi possiamo semplificare in:
$$-x(1-x)(x^2-x+1)$$
Allora calcoliamo il delta di $x^2-x+1$:
$$\Delta =1-4$$
Essendo minore di 0 non abbiamo radici reali.

Quindi le uniche radici (autovalori) del polinomio saranno $0,1$, essendo loro i valori che lo annullano.

Ora vogliamo risolvere per poter trovare gli autospazi $E(0)$ e $E(1)$:
$$E(1):=\begin{pmatrix}
0 & 1 & 0 & 0 \\
0 & 0 & -1 & 0 \\
1 & 2 & -2 & 0 \\
0 & 0 & 0 & 0
\end{pmatrix}\begin{pmatrix}
a_{0} \\
a_{1} \\
a_{2} \\
a_{3}
\end{pmatrix}=\begin{pmatrix}
0 \\
0 \\
0 \\
0 \\

\end{pmatrix}$$
Che una volta risolto darà come risultato:
$$\begin{cases}
a_{0}=2t \\
a_{1}=0 \\
a_{2}=t \\
a_{3}=t
\end{cases}$$
E allora l’ autospazio relativo a 1 sarà:
$$E(1)=\{2t+tx^2+tx^3\}$$
Invece l’ autospazio relativo a 0 avrà questo sistema:
$$\begin{pmatrix}
1 & 1 & 0 & 0 \\
0 & 1 & -1 & 1 \\
1 & 2 & -1 & 0 \\
0 & 0 & 0 & 1
\end{pmatrix}
\begin{pmatrix}
a_0 \\
a_1 \\
a_2 \\
a_3
\end{pmatrix}
=
\begin{pmatrix}
0 \\
0 \\
0 \\
0
\end{pmatrix}.$$
Che come risultato avrà:
$$E(0)=\{-t+tx+tx^2\}$$

Entrambi i sistemi hanno $dim=1$




Gli autovalori di un dato endomorfismo sono sempre uguali e non cambiano a seconda della base scelta, il motivo è spiegato nel suo [[Teorema sull’ invariabilità del polinomio caratteristico|teorema]]