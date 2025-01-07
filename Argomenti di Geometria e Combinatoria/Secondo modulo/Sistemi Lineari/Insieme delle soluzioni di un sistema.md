Sappiamo già che dato un sistema lineare [[Sistema Lineare Omogeneo|omogeneo]] avremo l’ insieme delle soluzioni $S$ come sottospazio vettoriale di $M(q,1,\mathbb{R})$.
Invece per quanto riguarda i sistemi lineari [[Sistema Lineare Omogeneo#Sistema lineare non omogeneo|non omogenei]], sappiamo che il loro insieme delle soluzioni $S$ non è considerabile sottospazio vettoriale.

Diamo quindi delle generalità sull’ insieme delle soluzioni di un sistema lineare $S$ non per forza omogeneo.

Prendiamo in esame il seguente sistema:
$$S:=\begin{cases}
x_1 + x_2 - x_3 + x_4 = 1 \\
2x_1 + x_2 - 3x_3 + 2x_4 = 0 \\
3x_1 + 2x_2 - 4x_3 + 3x_4 = 1 \\
5x_1 + 3x_2 - 7x_3 + 5x_4 = 1
\end{cases}

$$

Andiamo direttamente a trovare le soluzioni:
$$\begin{cases}
x_{1}=-1+2h-k \\
x_{2}=2-h \\
x_{3}=h \\
x_{4}=k
\end{cases}$$
Quindi scriviamo queste soluzioni come un insieme di matrici:
$$
\text{Sol}(S) = \left\{ 
\begin{pmatrix}
-1 + 2h - k \\
2 - h \\
h \\
k
\end{pmatrix}
\middle| h \in \mathbb{R}, k \in \mathbb{R}
\right\}.
$$
Notiamo subito che possiamo scomporre la soluzione: 
$$
\text{Sol}(S) = \left\{ 
\begin{pmatrix}
-1 + 2h - k \\
2 - h \\
h \\
k
\end{pmatrix}
= 
\begin{pmatrix}
-1 \\
2 \\
0 \\
0
\end{pmatrix}
+ h 
\begin{pmatrix}
2 \\
-1 \\
1 \\
0
\end{pmatrix}
+ k 
\begin{pmatrix}
-1 \\
0 \\
0 \\
1
\end{pmatrix}
\middle| h \in \mathbb{R}, k \in \mathbb{R}
\right\}
$$
Quindi abbiamo che l’ insieme $E$ formato dalle matrici
$$h \begin{pmatrix}
2 \\
-1 \\
1 \\
0
\end{pmatrix}
+ k \begin{pmatrix}
-1 \\
0 \\
0 \\
1
\end{pmatrix}$$
è l’ insieme delle combinazioni lineari delle matrici
$$\begin{pmatrix}
2 \\
-1 \\
1 \\
0
\end{pmatrix}
\ e\  
\begin{pmatrix}
-1 \\
0 \\
0 \\
1
\end{pmatrix}$$
<font color="#9bbb59">DUNQUE</font> $E$ è un sottospazio vettoriale di $M(4,1,\mathbb{R})$ di $dim=2$, pertanto abbiamo che:
$$Sol(S) = \begin{pmatrix}
-1 \\
2 \\
0 \\
0
\end{pmatrix}
+ E$$
<font color="#f79646">QUINDI</font>  Sol(S) è un sottospazio affine.

- Generalmente