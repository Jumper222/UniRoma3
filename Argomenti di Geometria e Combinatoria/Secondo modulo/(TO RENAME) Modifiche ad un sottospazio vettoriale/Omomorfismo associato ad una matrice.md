Siano dati $V,W$, due spazi vettoriali di dimensione <font color="#9bbb59">finita</font>.
Sia quindi data una <font color="#4bacc6">base</font>  per $V$ formata da $e_{1},e_{2},\dots,e_{n}$
Ed una <font color="#4bacc6">base</font> per $W$ formata da $f_{1},f_{2},\dots,f_{m}$
<font color="#f79646">Allora</font> esiste un unico <font color="#ffff00">omomorfismo</font> $f:V\to W$ la cui matrice rappresentativa rispetto le basi fissate è $A$ di tipo $M(m,n, R)$

 Per spiegare meglio il concetto facciamo un esempio:

1. Siano dati:
$$A:=\begin{cases}
1 & 0 & 1 \\
1 & 1 & 0 
\end{cases}$$
   - $e_{1}:=(1,1,1),e_{2}:=(1,1,0),e_{3}:=(1,0,0)$
   - $f_{1}:=(1,1),f_{2}:=(1,-1)$

2. Ricordandoci che il nostro obiettivo è trovare la legge che lega $f(x,y,z)$ ad ogni $(x,y,z)$ di $R^3$,
   calcoliamo le com