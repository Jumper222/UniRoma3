#Probabilità_e_statistica 
### <font color="#4bacc6">Esercizio</font>
Supponiamo di sapere che $X$ è una [[Variabili Aleatorie discrete e continue|v.a. continua]] con [[Fun. di densità di Probabilità (PDF)|PDF]]
$$f(x)\begin{cases}
C(4x-2x^2) & \quad 0<x<2 \\
0 & \quad \text{altrimenti}
\end{cases}$$
Chi deve essere $C$?

1. Innanzitutto studio le C.E. della equazione con $C$:
$$(4x-2x^2)>0\quad \forall x\in(0,2)$$
      E ovviamente $C>0$ altrimenti $f$ sarebbe negativa!
      
2. Iniziamo a calcolare l’ integrale tra questi due valori, ponendo l’ integrale uguale ad 1 perché l’ area della [[Fun. di densità di Probabilità (PDF)|PDF]] deve essere sempre uguale ad 1.
$$\int^\infty_{-\infty}f(x)dx=\int^2_{0}C(4x-2x^2)dx=1$$
$$C\int^2_{0}(4x-2x^2)dx=1$$
     Ora calcoliamo l’ integrale come fosse un normale integrale, e ci troveremo nella situazione:
     $$C\left( 8- \frac{16}{3} \right)=1$$
     $$C* \frac{8}{3}=1$$
     $$C=\frac{3}{8}$$
     Adesso sappiamo che $C$ assume il valore $\frac{3}{8}$

     Ora possiamo chiederci quanto vale $\mathbb{P}(X>1)$:
     $$\mathbb{P}(X>1)=\int^\infty_{1}f(x)dx=\int_{1}^2 \frac{3}{8}(4x-2x^2)dx$$
     Calcolando questo integrale normalmente avremo:
     $$\left[ 2x^2-\frac{2}{3}x^3 \right]^2_{1}$$
     E una volta risolto:
     $$\mathbb{P}(X>1)=\frac{1}{2}$$
3. Ora ci poniamo una 3° domanda: chi è $F$ (Ossia la [[Fun. di Ripartizione (CDF)|CDF]] di X)?
$$F(x)=\int^x_{-\infty}f(u)du=\begin{cases}
0  &  \text{se }x\leq 0 \\
\frac{3}{8}\left( 2x^2-\frac{2}{3}x^3 \right) & \text{se }x\in(1,2) \\
1 & \text{se }x\geq2 
\end{cases}$$
     Questo perché:
     - La probabilità che $X$ sia minore di un numero negativo è 0, perché $X$ può stare solo tra 0 e 2.
     - Il secondo termine appare nella forma $\int^x_{0} \frac{3}{8}(4u-2u^2)du$, che però abbiamo calcolato prima.
     - Invece nel secondo termine abbiamo 1 perché per valori superiori a quelli della curva il valore è fisso ad 1.

Finalmente possiamo descrivere questi due grafici

![[PDF Esempio.png]]
*Questo è il grafico della [[Fun. di densità di Probabilità (PDF)|PDF]], dove 3/4 è il punto di massimo calcolato con lo studio della derivata prima*.

![[Esempio CDF.png]]
*Questo è il grafico della [[Fun. di Ripartizione (CDF)|CDF]],*

<font color="#4bacc6">L’ esercizio è finito.</font>