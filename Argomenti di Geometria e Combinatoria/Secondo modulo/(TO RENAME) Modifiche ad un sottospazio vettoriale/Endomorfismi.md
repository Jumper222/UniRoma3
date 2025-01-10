#Geometria_e_Combinatoria 

Un <font color="#ffff00">endomorfismo</font> è un tipo particolare di omomorfismo che si ha quando lo spazio vettoriale di partenza è lo stesso dello spazio vettoriale di arrivo.

<font color="#f79646">Sostanzialmente</font>, un endomorfismo è rappresentato dalla sua matrice rappresentativa, che andrà a variare al variare delle basi scelte.

- Dato uno spazio vettoriale $V$, un <font color="#ffff00">endomorfismo</font> di $V$ è un omomorfismo $f:V\to V$


---

La <font color="#9bbb59">matrice rappresentativa</font> di un endomorfismo funziona allo stesso modo di quella di un omomorfismo, facciamo un esempio:

Sia dato l’ omomorfismo $f:R^3[x]\to R^3[x]$:
$f(a+bx+cx^2):=(3a+c)+(a+b)x+c\ x^2$

Ora determiniamo le immagini dei vettori di $f$ rispetto la base canonica, e poi li decomponiamo:

- $f(1)=3+x=\phantom{00}3\ 1 +1 \ x+0\ x^2$
- $f(x)=x=\phantom{33333}0\ 1+1\ x+0 x^2$
- $f(x^2)=1+x^2=1\ 1+0\ x+ 1\ x^2$

Allora la mat. rappresentativa di $f$ rispetto la base canonica sarà:

$$\begin{pmatrix}
3 & 0 & 1 \\
1 & 1  & 0\\
0 & 0 & 1
\end{pmatrix}$$
Gli endomorfismi hanno un legame molto stretto con il [[Cambio di base|cambio di base]]