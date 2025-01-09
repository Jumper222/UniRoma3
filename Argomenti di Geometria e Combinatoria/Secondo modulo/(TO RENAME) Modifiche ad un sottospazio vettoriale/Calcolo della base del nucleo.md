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
