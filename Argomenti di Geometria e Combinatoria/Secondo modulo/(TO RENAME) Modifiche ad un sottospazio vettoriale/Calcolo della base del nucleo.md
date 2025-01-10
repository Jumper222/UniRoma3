#Geometria_e_Combinatoria 
Riflettiamo meglio su cosa stiamo cercando:
Dato un <font color="#ffff00">omomorfismo</font> $f:V\to W$, data una base per $V$ formata da $v_{1},v_{2},\dots,v_{n}$
ed una base per $W$ formata da $w_{1},w_{2},\dots,w_{m}$

Sia $A$ allora la matrice rappresentativa di $f$ rispetto le basi date.
Consideriamo ora un generico vettore $v$, che vogliamo stabilire se appartiene a $ker\ f$
Avremo quindi $v:$
$$v:=x_{1}e_{1}+x_{2}e_{2}+\dots+x_{n}e_{n}$$
Per determinare se tale vettore appartiene al nucleo dovremo assicurarci che
$$f(v)=y_{1}f_{1}+y_{2}f_{2}+\dots+y_{m}f_{m}$$
E allora vogliamo avere tutti i valori $y=0$


---

Facciamo un esempio per capire meglio:

### <font color="#4bacc6">Esempio 1</font>

Sia l’ omomorfismo $f:V\to W$, con $e_{1},e_{2},e_{3},e_{4}$ come base di $V$ e $f_{1},f_{2},f_{3}$ come base di $W$ t.c:
- $f(e_{1}):=f_{1}+f_{2}+f_{3}$
- $f(e_{2}):=f_{1}+2f_{2}+3f_{3}$
- $f(e_{3}):=3f_{1}+4f_{2}+5f_{3}$
- $f(e_{4}):=-f_{2}-2f_{3}$

E abbiamo quindi la matrice rappresentativa:

$$A:=\begin{pmatrix}
1 & 1 & 3 & 0 \\
1 & 2 & 4 & -1 \\
1 & 3 & 5 & -2
\end{pmatrix}$$
Che quindi possiamo ridurre a scalini:
$$A'=\begin{pmatrix}
1 & 1 & 3 & 0 \\
0 & 1 & 1 & -1 \\
0 & 0 & 0 & 0
\end{pmatrix}$$
Quindi lo <font color="#ffff00">moltiplichiamo</font> con il vettore di incognite, che ha <font color="#f79646">4 valori</font> perché sono 4 le dimensioni dello spazio vettoriale di partenza, e cerchiamo come risultato un <font color="#4bacc6">vettore</font> nullo di grandezza 3, ovvero le dimensioni del sistema di arrivo.

$$\begin{pmatrix}
1 & 1 & 3 & 0 \\
0 & 1 & 1 & -1 \\
0 & 0 & 0 & 0
\end{pmatrix}\begin{pmatrix}
x \\
y \\
z \\
w
\end{pmatrix}=\begin{pmatrix}
0 \\
0 \\
0
\end{pmatrix}$$
Risolviamo quindi e troviamo il vettore $(-2t-u,-t+u,t,u)$. Allora poniamo prima $t=1,u=0$ e poi $t=0,u=1$

Allora avremo le basi per $ker\ f$:
$$ker\ f: -2e_{1}-1e_{2}+1e_{3}+0e_{4};-1e_{1}+1e_{2}+0e_{3}+1e_{4}$$
### <font color="#4bacc6">Esempio 2</font>

Sia l’ omomorfismo $f:R^3\to R^4[x]$, definito da:
$$f(a,b,c):=(2a+b+8c)+(3a-b+7c)x+(-a-3c)x^2+(b+2c)x^3$$
Troviamo allora la matrice rappresentativa:
$$A:=\begin{pmatrix}
2 & 1 & 8 \\
3 & -1 & 7 \\
-1 & 0 & -3 \\
0 & 1 & 2
\end{pmatrix}$$
Quindi riduciamola a scalini: 
$$\begin{pmatrix}
2 & 1 & 8 \\
0 & -\frac{5}{2} & 5 \\
0 & 0 & 0 \\
0 & 0 & 0
\end{pmatrix}\begin{pmatrix}
x_{1} \\
x_{2} \\
x_{3}
\end{pmatrix}=\begin{pmatrix}
0 \\
0 \\
0 \\
0
\end{pmatrix}$$
Da calcoliamo il risultato che è uguale a:
$$(-3t,-2t,t)$$
E allora sappiamo che la base di $ker\ f$ è uguale a $(-3,-2,1)$
