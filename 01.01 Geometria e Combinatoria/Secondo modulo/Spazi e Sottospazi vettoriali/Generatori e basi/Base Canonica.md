#Geometria_e_Combinatoria 
Una <font color="#ffff00">base canonica</font> è una base definita per l’insieme $\mathbb{R}^n$:
$\{e_{1},e_{2},\dots,e_{n}\}$
formato dai seguenti vettori:
$e_{1}=(1,0,0,\dots,0)$
$e_{2}=(0,1,0,\dots,0)$
$e_{n}=(0,0,0,\dots,1)$

Ossia, in termini semplici una <font color="#ffff00">base canonica</font> è un generatore formato da dei vettori $e$ che come unico valore possiedono un 1 nella loro posizione rispetto al generatore.

Ogni vettore $v=v_{1},v_{2},\dots,v_{r}\in\mathbb{R}$ può quindi essere descritto come combinazione lineare dei vettori della <font color="#ffff00">base canonica</font>.

Facciamo ora un esempio di una base canonica:


### <font color="#4bacc6">Esempio di base canonica</font>
Siano date le seguenti matrici all’ interno di $M(3,2,R)$:
$$E_{11}:=\begin{pmatrix}
1&0 \\
0&0 \\
0&0
\end{pmatrix},\quad E_{12}:=\begin{pmatrix}
0&1 \\
0&0 \\
0&0
\end{pmatrix}, \quad E_{21}:=\begin{pmatrix}
0&0 \\
1&0 \\
0&0
\end{pmatrix},
\quad E_{22}:=\begin{pmatrix}
0&0 \\
0&1 \\
0&0
\end{pmatrix} \quad E_{31}:=\begin{pmatrix}
0&0 \\
0&0 \\
1&0
\end{pmatrix} \quad E_{32}:=\begin{pmatrix}
0&0 \\
0&0 \\
0&1
\end{pmatrix}$$
Allora  se volessimo descrivere la matrice $$A=\begin{pmatrix}
a&b \\
c&d \\
e&f
\end{pmatrix}$$
La descriveremo:
$$A=aE_{11}+bE_{12}+cE_{21}+dE_{22}+eE_{31}+fE_{32}$$
Quindi le 6 matrici sono linearmente indipendenti e formano una base (canonica) di $M(3,2,R)$

- Da questo esempio possiamo trarre una utile osservazione: una base per $M(p,q,R)$ è formata dalle $pq$ matrici $E_{ij}$ dove $E_{ij}$ è la matrice in cui tutti gli elementi sono 0 tranne quello di posto $(i,j)=1$

- Inoltre, data una base canonica per l’ insieme delle matrici, allora qualsiasi matrice all’ interno di tale insieme potrà essere descritta usando gli elementi della matrice stessa.


