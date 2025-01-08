#Geometria_e_Combinatoria 
Consideriamo un sistema lineare omogeneo SO definito come $AX=0$ di $p$ equazioni in $q$ incognite $x_{1},x_{2},\dots,x_{q}$
Sia $rk \ A=r$, allora lo spazio delle soluzioni Sol(SO) ha $dim \ q-r$

Per comprendere al meglio questo concetto, facciamo un esempio.

### <font color="#4bacc6">Esempio</font> (fare attenzione a tutti i passaggi)
Sia dato il seguente sistema:
$$\begin{cases}
2x-4y+\phantom{2}z-w-2t&=0 \\
\phantom{2}x-2y-2z+w&=0 \\
3x-6y-\phantom{2}z\phantom{-w_{2}}-2t&=0
\end{cases}$$
Per poter conoscere $dim \ Sol(SO)$ prima bisogna risolverlo, per farlo useremo l’ eliminazione Gaussiana, come prima cosa leviamo $-\frac{1}{2}*I \ riga$ alla seconda riga:
$$\begin{cases}
2x-4y+\phantom{\frac{5}{2}}z-\phantom{\frac{3}{2}}w-2t&=0 \\
\phantom{2x-2y}-\frac{5}{2}z+\frac{3}{2}w+\phantom{1}t&=0 \\
3x-6y-\phantom{\frac{5}{2}}z\phantom{---}-2t&=0
\end{cases}$$
Come seconda cosa leviamo $-\frac{3}{2} * I \ riga$ alla terza riga:
$$\begin{cases}
2x-4y+\phantom{\frac{5}{2}}z-\phantom{\frac{3}{2}}w-2t&=0 \\
\phantom{2x-2y}-\frac{5}{2}z+\frac{3}{2}w+\phantom{1}t&=0 \\
\phantom{2x-2y}-\frac{5}{2}z+\frac{3}{2}w+\phantom{1}t&=0
\end{cases}$$
Essendo ora la 2° e la terza riga identiche, possiamo sottrarre la 3° riga alla seconda ed avremo risolto il sistema.
$$\begin{cases}
2x-4y+\phantom{\frac{5}{2}}z-\phantom{\frac{3}{2}}w-2t&=0 \\
\phantom{2x-2y}-\frac{5}{2}z+\frac{3}{2}w+\phantom{1}t&=0 \\
\phantom{2x-2y-\frac{5}{2}z+\frac{3}{2}w+3}0&=0
\end{cases}$$
Ora bisogna prestare <font color="#f79646">moltissima</font> attenzione:

Assegniamo a $w$ e $t$ i valori parametrici $h_{2},h_{3}$, questo perché mancano 2 “scalini” perché diventi una matrice triangolare.
Fatto ciò risolviamo $z$ in funzione di $w$ e $t$, $z=\frac{3}{5}h_{2}+\frac{2}{5}h_{3}$
Ora assegniamo a $y$ il valore parametrico $h_{1}$ e quindi risolviamo per $x$ la equazione:
$x=2h_{1}+\frac{1}{5}h_{2}+\frac{4}{5}h_{3}$

Il sistema risolto quindi sarà:

$$\begin{cases}
x=2h_{1}+\frac{1}{5}h_{2}+\frac{4}{5}h_{3} \\
y=\phantom{1}h_{1} \\
z=\phantom{2h_{3}3+}\frac{3}{5}h_{2}+\frac{2}{5}h_{3} \\
w=\phantom{22222_{22}}h_{2} \\
t=\phantom{22222222222_{222}}h_{3}
\end{cases}$$
Quindi possiamo scrivere le soluzioni come matrici di M(5,1,R):
$$Sol(SO)=\begin{pmatrix}
2h_{1}+\frac{1}{5}h_{2}+\frac{4}{5}h_{3}  \\
h_{1} \\
\frac{3}{5}h_{2}+\frac{2}{5}h_{3} \\
h_{2} \\
h_{3}

\end{pmatrix}
$$
Descrivibile anche come:

$$Sol(SO)= \left\{h_{1}\begin{pmatrix}
2 \\
1 \\
0 \\
0 \\
0
\end{pmatrix}+h_{2}\begin{pmatrix}
\frac{1}{5} \\
0 \\
\frac{3}{5} \\
1 \\
0
\end{pmatrix}+h_{3}\begin{pmatrix}
\frac{4}{5} \\
0 \\
\frac{2}{5} \\
0 \\
1
\end{pmatrix}\right\}$$
E quindi possiamo finalmente dire che Sol(SO) è generato da $S_{1},S_{2},S_{3}$:
$$S_{1}:=\begin{pmatrix}
2 \\
1 \\
0 \\
0 \\
0
\end{pmatrix},\quad S_{2}:=\begin{pmatrix}
\frac{1}{5} \\
0 \\
\frac{3}{5} \\
1 \\
0
\end{pmatrix},\quad S_{3}:=\begin{pmatrix}
\frac{4}{5} \\
0 \\
\frac{2}{5} \\
0 \\
1
\end{pmatrix}$$
Quindi stabiliamo se essi formano una base per Sol(SO), verificando se sono linearmente indipendenti: $h_{1}S_{1}+h_{2}S_{2}+h_{3}S_{3}=0$
$$\begin{pmatrix}
2h_{1}+\frac{1}{5}h_{2}+\frac{4}{5}h_{3} \\
h_{1} \\
\frac{3}{5}h_{2}+\frac{2}{5}h_{3} \\
h_{2} \\
h_{3}
\end{pmatrix}=\begin{pmatrix}
0 \\
0 \\
0 \\
0 \\
0
\end{pmatrix}$$
Ovviamente questa uguaglianza si verifica solo quando $h_{1}=h_{2}=h_{3}=0$.

- <font color="#9bbb59">Si ha quindi</font> che $S_{1},S_{2},S_{3}$ sono una base di Sol(SO), e che esso ha $dim=3$