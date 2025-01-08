#Geometria_e_Combinatoria 
Tra le applicazioni $f:V\to W$ tra due spazi vettoriali sono particolarmente importanti gli <font color="#ffff00">Omomorfismi</font>:

Allora iniziamo a definire cosa è un omomorfismo:
Esso è un tipo particolare di funzione tra spazi vettoriali tale che valgono le seguenti proprietà:
- $f(u+v)=f(u)+f(v)$, per ogni $u\in V, \ v\in V$
- $f(ku)=kf(u)$ per ogni $k\in \mathbb{R},u\in V$

Per stabilire se una applicazione sia o meno un <font color="#ffff00">omomorfismo</font> ci sarà utile dare dei nomi alle proprietà, quindi diremo che:
- $f$ <font color="#00b050">rispetta l’ addizione</font> se soddisfa la 1° proprietà
- $f$ <font color="#00b050">rispetta la moltiplicazione</font> se soddisfa la 2° proprietà

Facciamo un banale esempio:
- Se $V$ e $W$ sono due spazi vettoriali, è facile vedere che l’ applicazione $f:V \to W$ che associa ad ogni vettore di $V$ il vettore nullo di $W$ è un <font color="#ffff00">omomorfismo</font>, esso è infatti detto <font color="#ffff00">omomorfismo nullo</font>.

Facciamo degli [[Esempi sugli Omomorfismi|esempi]] più complessi per comprendere meglio


Una volta capito cosa è un omomorfismo possiamo concentrarci sul come trovare la [[Matrice associata ad un omomorfismo|matrice associata ad un omomorfismo]], ed anche la sua operazione inversa, ovvero trovare l’ [[Omomorfismo associato ad una matrice|omomorfismo associato ad una matrice]]

### Possibili esercizi:
#### Stabilire  la linearità:

Potrebbero capitare degli <font color="#9bbb59">esercizi</font> dove si cerca di stabilire la <font color="#ffff00">linearità</font> di un dato omomorfismo,
Essi sono <font color="#f79646">facilmente</font> risolubili con una semplice regola, le espressioni all’ interno dell’ omomorfismo devono essere polinomi omogeni di primo grado, ossia:
$$0,-x,2x-y$$
è l’ esempio <font color="#ffff00">perfetto</font>.

Alcuni esempi errati:
- $2x-y+1$ <font color="#d99694">non</font> è omogeneo perché c’è l’1
- $xy$ <font color="#d99694">non</font> è di primo grado, ma di secondo.


#### Stabilire l’ esistenza di omomorfismi:
Data una legge $f$ e un tot di <font color="#4bacc6">vettori</font> appartenenti all’ insieme di partenza,
Se essi stabiliscono una base per l’insieme di <font color="#ffff00">partenza</font> allora possiamo dire che esiste un solo <font color="#f79646">omomorfismo</font> che soddisfa le condizioni date:

Dati:
- $f:R^3\to R^2$
- $f(1,2,1)=(0,1)$
- $f(1,0,2)=(0,1)$
- $f(2,2,1)=(2,1)$

Li poniamo in una matrice:
$$\begin{pmatrix}
1 & 1 & 2 \\
2 & 0 & 2 \\
1 & 2 & 1
\end{pmatrix}$$
Notiamo subito che essi <font color="#9bbb59">formano</font> una base per $R^3$, avendo il det. <font color="#d99694">non</font> nullo.
Se essi avessero avuto un det. nullo allora non sarebbe esistito nessun omomorfismo.

È utile ricordare cosa è l’ [[Immagine di un omomorfismo]]