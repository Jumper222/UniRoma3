#Probabilità_e_statistica 
Alcune volte potremmo dover calcolare il [[Valore Atteso]] di una variabile aleatoria in funzione di un’ altra variabile aleatoria.
Per nostra fortuna il processo non è per nulla difficile e con un semplice esempio si potranno capire tutte le intricatezze:

Esempio: Il tempo necessario ad identificare (e sistemare) un guasto in una fabbrica (in ore) è modellizzato da una v.a. X con PDF:

$$f_{X}(x)=\begin{cases}
1 & \text{se }x\in[0,1] \\
0 & \text{altrimenti}
\end{cases}=F_{X}(x)=\begin{cases}
0 & \text{se }x<0 \\
x & \text{se }x\in[0,1] \\
1 & \text{se }x>1 
\end{cases}$$
Se il danno economico provocato da un interruzione di $x$ ore è $x^3$, qual’è il valore attesto del danno provocato da un guasto?

Innanzitutto definiamo la v.a. $Y=X^3$, che rappresenta il danno provocato da un guasto
Ora ci domandiamo come è distribuita $Y$ e quale sia la sua CDF.
Ovviamente $\mathrm{Im}(Y)=\mathrm{Im}(X^3)=[0,1]$
Allora $F_{Y}(y)=0\quad \forall y\leq0$, mentre
$\forall y\in$$
