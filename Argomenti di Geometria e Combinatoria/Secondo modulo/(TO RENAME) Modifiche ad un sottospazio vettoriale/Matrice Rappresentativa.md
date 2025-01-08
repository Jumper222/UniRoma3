#Geometria_e_Combinatoria 
La <font color="#ffff00">matrice rappresentativa</font> di un omomorfismo è la matrice che, quando moltiplicata per un vettore espresso rispetto a una base dell'insieme di partenza produce il vettore immagine nell'insieme di arrivo, espresso rispetto a una base dell'insieme di arrivo. Per spiegare bene cosa è la matrice rappresentativa, studiamo meglio un [[Esempi sugli Omomorfismi|esempio]] già fatto in precedenza:


Sia $f:R^3\to R^2$ l’ omomorfismo t.c: $f(x,y,z)=(x+y,y+z)$

1. Formiamo una <font color="#f79646">base</font> di $R^3$: 
   $e_{1}:=(1,0,0)$
   $e_{2}:=(1,1,0)$
   $e_{3}:=(1,1,1)$
2. Ora formiamo una <font color="#f79646">base</font> di $R^2$:
   $f_{1}:=(1,1)$
   $f_{2}:=(2,1)$
3. Determiniamo la matrice rappresentativa di $f$ rispetto queste basi:
   $f(e_{1})=f(1,0,0)=(1,0)$
   $f(e_{2})=f(1,1,0)=(2,1)$
   $f(e_{3})=f(1,1,1)=(2,2)$
4. Ora <font color="#9bbb59">decomponiamo</font> le immagini rispetto la base composta da $f_{1}$ ed $f_{2}$, ossia troviamo dei valori scalari $a,b$ che moltiplicati per la base diano come risultato la base che noi abbiamo trovato dell’ insieme di arrivo
   $f(e_{1})=(1,0)=a(1,1)+b(2,1)$
   $f(e_{2})=(2,1)=a(1,1)+b(2,1)$
   $f(e_{3})=(2,2)=a(1,1)+b(2,1)$
5. Per fare ciò potrebbe risultare utile scomporre in un sistema le immagini di $e_{1},e_{2},e_{3}$:
$$f(e_{1})=(1,0):\begin{cases}
a + 2b = 1 \\
a + b = 0
\end{cases}$$
$$f(e_{2})=(2,1):\begin{cases}
a + 2b = 2 \\
a + b = 1
\end{cases}$$
$$f(e_{3})=(2,2):\begin{cases}
a + 2b = 2 \\
a + b = 2
\end{cases}$$
6. Ora risolviamo i sistemi e troviamo che:
   Per $f_{1}, \ a=-1,b=1$
   Per $f_{2},a=0,b=1$
   Per $f_{3},a=2,b=0$
7. Infine creiamo la matrice rappresentativa, piazzando $a$ di sopra e $b$ di sotto:
$$A:=\begin{pmatrix}
-1 & 0 & 2 \\
1 & 1 & 0
\end{pmatrix}$$

- Ora che abbiamo la matrice rappresentativa possiamo prendere un qualsiasi <font color="#f79646">vettore</font> $v$ e moltiplicarlo per quest’ultima per avere il risultato della applicazione lineare:

8. Prendiamo il vettore $v:=(2e_{1}+3e_{2}-1e_{3})$ e moltiplichiamolo per $A$:
$$\begin{pmatrix}
-1 & 0 & 2 \\
1 & 1 & 0
\end{pmatrix}
\begin{pmatrix}
2 \\
3 \\
-1
\end{pmatrix}
=
\begin{pmatrix}
-4 \\
5
\end{pmatrix}$$
9. Quindi troviamo $f(v)=-4f_{1}+5f_{2}$, che se quindi moltiplicata ad $f_{1}$ ed $f_{2}$ troveremo l’ immagine di $v$:
$$-4f_{1}+5f_{2}=-4(1,1)+5(2,1)=(6,1), \quad\quad\quad f(v)=6,1$$




<font color="#f79646">Nota bene</font>: La matrice rappresentativa di una applicazione è legata alle basi scelte, quindi una applicazione avrà sempre varie matrici rappresentative.
<font color="#f79646">Nota bene</font>: Se per descrivere la matrice rappresentativa usassimo<font color="#ffff00"> solo basi canoniche</font> avremmo una matrice molto particolare, con delle colonne che danno $f(e_{1})$,$f(e_{2})$,$f(e_{3})$, e con delle righe che corrispondono ai coefficienti di $x,y,z$ nelle espressioni $x+y$ e $y+z$ se rifacessimo l’ esempio appena discusso con le basi canoniche avremmo:
$f(e_{1})=f(1,0,0)=(1,0)=f_{1}$
$f(e_{2})=f(0,1,0)=(1,1)=f_{1}+f_{2}$
$f(e_{3})=f(0,0,1)=(0,1)=f_{2}$

$$A:=\begin{cases}
1 & 1 & 0 \\
0 & 1 & 1
\end{cases}$$