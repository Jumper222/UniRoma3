Data una matrice  $A\ (n\times n)$, 
Il polinomio caratteristico $p(\lambda)$ è un polinomio di grado $n$ in $\lambda$, ossia con variabili $\lambda$.
Ed è definito come determinante della matrice $A-\lambda I$, ossia:
$$p(\lambda)=\det(A-\lambda I)$$

Serve quindi per trovare gli autovalori, risolvendo l’ equazione:
$$\det(A-\lambda I)=0$$
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
\phantom{123}a_1 - a_2 + a_3 &= \lambda a_1 \\
a_0 + 2a_1 - a_2 &= \lambda a_2 \\
\phantom{a_0 + 2a_1+1+} a_3 &= \lambda a_3
\end{cases}$$