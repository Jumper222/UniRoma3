#Geometria_e_Combinatoria 
### <font color="#4bacc6">Esempio 1</font>

Sia $f:M(2,2,R)\to M(2,2,R)$ definito da $f(A):=A+A^t$.
Per determinare $ker\ f$ possiamo considerare la matrice generica di $M(2,2,R)$:
$$A:=\begin{pmatrix}
x & y \\
z & w
\end{pmatrix}$$
Poi gli applichiamo l’ omomorfismo:
$$f(A)=\begin{pmatrix}
x & y \\
z & w
\end{pmatrix}+
\begin{pmatrix}
x & y \\
z & w
\end{pmatrix}^t=\begin{pmatrix}
2x & y+z \\
y+z & 2w
\end{pmatrix}$$
Quindi impostiamo il sistema lineare omogeneo:
$$\begin{cases}
2x &= 0 \\
\phantom{2x+}y + z &= 0 \\
\phantom{2x+}y + z &= 0 \\
\phantom{2x+y+z} 2w &= 0
\end{cases}\to ker\ f=\begin{pmatrix}
0 & t \\
-t & 0
\end{pmatrix}$$
Quindi possiamo dire che $ker \ f$ è un sottospazio vettoriale dell’ insieme di partenza.
Si può inoltre notare che $ker\ f$ è formato dalle matrici $A$ tali che $A+A^t=0$, cioè le matrici <font color="#f79646">antisimmetriche</font> tali che $A^t=-A$