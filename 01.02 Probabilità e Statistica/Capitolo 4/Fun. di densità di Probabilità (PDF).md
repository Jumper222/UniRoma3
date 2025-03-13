#Probabilità_e_statistica 
>[!Definizione]  Definizione
>La [[Funzioni|funzione]] di densità di probabilità (PDF) è come se fosse l’ analogo della [[Fun. di massa di Probabilità (PMF)|PMF]] però per le [[Variabili Aleatorie|v.a.]] [[Variabili aleatorie discrete e continue|continue]]
>Essa assegna una densità della probabilità, però la probabilità di un singolo valore è sempre 0, e la formula è:
>$$\mathbb{P}(X\leq a)=F(a)=\int^a_{-\infty}f(x)dx$$
>Nota:
>- $f(x)\geq0 \quad \forall x$
>- L’ area totale sotto la curva è sempre 1.
>Per poter usare questa funzione sostituiamo gli estremi di integrazione con i valori tra cui stiamo calcolando la probabilità.

---
Facciamo un esempio:

Abbiamo $X$ che è il primo istante di tempo in cui si rompe la mia auto a partire da ora (Chiaramente è una v.a. <font color="#ffff00">continua</font>)
Allora abbiamo i casi: (Prendiamo $F \sim X$)
$$F(x)=\begin{cases}
0  & \text{se }x<0 \\
1-e^{-2x} & \text{se }x\geq0
\end{cases}$$
![[PDF.png]]
- [I] <font color="#ffff00">Questo è un grafico che rappresenta la CDF di una funzione continua</font>
 
Quindi quando x supera 0 inizia ad avere un comportamento come $1-e^{-2x}$
Allora la funzione sarà nella forma:
$$f(x)=\begin{cases}
0 & \text{se }x<0 \\
2e^{-2x} & \text{se }x\geq 0
\end{cases}$$
E quindi avremo questo grafico:
![[Esempio PDF.png]]

E come si può vedere nella seconda immagine questo grafico sarà lo strumento che useremo per la PDF