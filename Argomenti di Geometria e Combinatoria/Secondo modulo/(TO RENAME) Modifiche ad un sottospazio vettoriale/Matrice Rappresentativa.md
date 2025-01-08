La matrice rappresentativa di un omomorfismo è la matrice che, quando moltiplicata per un vettore espresso rispetto a una base dell'insieme di partenza produce il vettore immagine nell'insieme di arrivo, espresso rispetto a una base dell'insieme di arrivo. Per spiegare bene cosa è la Matrice rappresentativa, studiamo meglio un [[Esempi sugli Omomorfismi|esempio]] già fatto in precedenza:


Sia $f:R^3\to R^2$ l’ omomorfismo t.c: $f(x,y,z)=(x+y,y+z)$

1. Formiamo una base di $R^3$: 
   $e_{1}:=(1,0,0)$
   $e_{2}:=(1,1,0)$
   $e_{3}:=(1,1,1)$
2. Ora formiamo una base di $R^2$:
   $f_{1}:=(1,1)$
   $f_{2}:=(2,1)$
3. Determiniamo la matrice rappresentativa di $f$ rispetto queste basi:
   $f(e_{1})=f(1,0,0)=(1,0)$
   $f(e_{2})=f(1,1,0)=(2,1)$
   $f(e_{3})=f(1,1,1)=(2,2)$
4. Ora decomponiamo le immagini rispetto la base composta da $f_{1}$ ed $f_{2}$, ossia troviamo dei valori scalari $a,b$ che moltiplicati per la base diano come risultato la base che noi abbiamo trovato dell’ insieme di arrivo
   $f(e_{1})=(1,0)=a(1,1)+b(2,1)$
   $f(e_{2})=(2,1)=a(1,1)+b(2,1)$
   $f(e_{3})=(2,2)=a(1,1)+b(2,1)$
5. Per fare ciò potrebbe risultare utile scomporre in un sistema le immagini di $e_{1},e_{2},e_{3}$:
$$f(e_{1})=(1,0):\begin{cases}
a + 2b = 1 \\
a + b = 0
\end{cases}$$
$$$$