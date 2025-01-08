#Geometria_e_Combinatoria 
Per Immagine di un <font color="#ffff00">omomorfismo</font> si intende un insieme all’ interno dell’ insieme di arrivo che contiene tutti gli elementi immagine della legge. Solitamente ha delle regole o condizioni particolari, che rispettano quelle dell’ <font color="#ffff00">omomorfismo</font>.

Facciamo un esempio:

Dato l’ <font color="#ffff00">omomorfismo</font> $f:R^2\to R^3$, definito da: $f(x,y):=(x+2y,x+y,x-y)$.
L’ insieme immagine sarà quindi composto da tutti quei <font color="#4bacc6">vettori</font> $w:=(a,b,c)$ di $R^3$ per cui esiste un <font color="#4bacc6">vettore</font> $v:=(x,y)$ di $R^2$ tale che $f(v)=w$, ossia $(x+2y,x+y,x-y)=(a,b,c)$. Andiamo quindi a scrivere questo sistema:
$$\begin{cases}
x+2y=a \\
x+y=b \\
x-y=c
\end{cases}\to \begin{cases}
x+2y=a \\
-y=a-b \\
0=2a-3b+c
\end{cases}$$
- Abbiamo quindi che questo sistema è risolubile se e solo se $0=2a-3b+c$
- Possiamo allora descrivere l’ insieme immagine di questo omomorfismo:
$$f(\mathbb{R}^{2})=\{(a,b,c)|2a-3b+c=0\}$$
- I vettori che quindi appartengono a questo sottoinsieme sono tutti immagini di $f$.

<font color="#f79646">Attenzione</font>:nonostante l’ insieme immagine sia interno ad uno spazio vettoriale, non è detto che esso stesso sia un sottospazio vettoriale, in quanto potrebbe come potrebbe non verificare le proprietà dei sottospazi vettoriali, bisogna quindi valutare caso per caso.

---

Facciamo ora un esempio di come calcolare la base dell’immagine di un omomorfismo:


Sia $V$ uno spazio vettoriale con base formata da $e_{1},e_{2},e_{3},e_{4}$
Sia $W$ uno spazio vettoriale con base formata dai vettori $f_{1},f_{2},f_{3}$.
Sia $f:V\to W$ l’ omomorfismo t.c:
- $f(e_{1})=f_{1}+f_{2}+f_{3}$
- $f(e_{2})=f_{1}+2f_{2}+3f_{3}$
- $f(e_{3})=3f_{1}+4f_{2}+5f_{3}$
- $f(e_{4})=-f_{2}-2f_{3}$

Per determinare la base dell’ immagine di $f$ consideriamo la matrice con colonne le componenti di $f_{1},f_{2},f_{3},f_{4}$

$$A := \begin{pmatrix}
1 & 1 & 3 & 0 \\
1 & 2 & 4 & -1 \\
1 & 3 & 5 & -2
\end{pmatrix}$$
Fatto ciò la riduciamo a scalini:
$$B := \begin{pmatrix}
1 & 1 & 3 & 0 \\
0 & 1 & 1 & -1 \\
0 & 0 & 0 & 0
\end{pmatrix}$$
Ora vediamo dove appaiono gli “scalini”, ovvero in prima e seconda posizione.
- Da qui troviamo la base per $f(V)$, che è quindi data da $f(e_{1}),f(e_{2})$: $f_{1}+f_{2}+f_{3},f_{1}+2f_{2}+3f_{3}$

<font color="#f79646">Nota bene</font>: 