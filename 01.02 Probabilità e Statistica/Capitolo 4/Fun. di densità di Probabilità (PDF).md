#Probabilità_e_statistica 
>[!Definizione]  Definizione
>La [[Funzioni|funzione]] di densità di probabilità (PDF) è come se fosse l’ analogo della [[Fun. di massa di probabilità (PMF)|PMF]] però per le [[Variabili Aleatorie|v.a.]] [[Variabili aleatorie discrete e continue|continue]]
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