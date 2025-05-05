#Probabilità_e_statistica 
Alcune volte potremmo dover calcolare il [[Valore Atteso]] di una variabile aleatoria in funzione di un’ altra variabile aleatoria.
Per nostra fortuna il processo non è per nulla difficile e con un semplice esempio si potranno capire tutte le intricatezze:

Esempio: Il tempo necessario ad identificare (e sistemare) un guasto in una fabbrica (in ore) è modellizzato da una [[Variabili Aleatorie|v.a.]] X con PDF:

$$f_{X}(x)=\begin{cases}
1 & \text{se }x\in[0,1] \\
0 & \text{altrimenti}
\end{cases}=F_{X}(x)=\begin{cases}
0 & \text{se }x<0 \\
x & \text{se }x\in[0,1] \\
1 & \text{se }x>1 
\end{cases}$$
Se il danno economico provocato da un interruzione di $x$ ore è $x^3$, qual’è il valore attesto del danno provocato da un guasto?

Innanzitutto definiamo la [[Variabili Aleatorie|v.a.]] $Y=X^3$, che rappresenta il danno provocato da un guasto
Ora ci domandiamo come è distribuita $Y$ e quale sia la sua [[Fun. di Ripartizione (CDF)|CDF]].
Ovviamente $\mathrm{Im}(Y)=\mathrm{Im}(X^3)=[0,1]$
Allora $F_{Y}(y)=0\quad \forall y\leq0$, mentre
$$\forall y\in[0,1]\quad F_{Y}(y)=\mathbb{P}(Y\leq y)=\mathbb{P}(X^3\leq y)$$
 ne consegue:
 $$\mathbb{P}(X\leq y^{1/3})=F_{X}(y^{1/3})=\int^{y^{1/3}}_{0}f_{x}(x)dx=(x)^{y^{1/3}}_{0} =y^{1/3}$$
 E allora la sua CMF sarà nella forma:
$$F_{Y}(y)=\begin{cases}
0 & \text{se }y<0 \\
y^{1/3} & \text{se }y\in[0,1] \\
1 & \text{se }y>1
\end{cases}$$
![[CMF valore attesto di una variabile aleatoria composta.png]]

Per trovare $f_{Y}$ sarà sufficiente derivare $F_{Y}$:
$$F_{Y}'=\frac{1}{3}y^{-2/3}$$
![[PDF valore atteso di una v.a. composta.png]]
*PDF di Y e X sovrapposte*

Allora possiamo calcolare facilmente il [[Valore Atteso]] di $Y$:
$$\mathbb{E}[Y]=\int_{0}^1y\ f_{Y}(y)dy=\int_{0}^1 \frac{1}{3}y^{1/3}dy=\dots=\frac{1}{4}$$
<font color="#f79646">NB</font>: alternativamente avremmo potuto calcolare il [[Valore Atteso]] direttamente da $X^3$
$$\mathbb{E}[Y]=\mathbb{E}[X^3]=\int_{0}^1x^3f_{X}(x)dx=\int_{0}^1x^3dx=\frac{1}{4}$$

Se volessimo generalizzare questa nozione diremmo che questo è il momento n-esimo di X, con n=3