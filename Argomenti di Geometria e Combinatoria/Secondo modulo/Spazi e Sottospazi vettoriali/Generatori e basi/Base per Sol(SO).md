Consideriamo un sistema lineare omogeneo SO definito come $AX=0$ di $p$ equazioni in $q$ incognite $x_{1},x_{2},\dots,x_{q}$
Sia $rk \ A=r$, allora lo spazio delle soluzioni Sol(SO) ha $dim \ q-r$

Per comprendere al meglio questo concetto, facciamo un esempio.

### <font color="#4bacc6">Esempio</font> (fare attenzione a tutti i passaggi)
Sia dato il seguente sistema:
$$\begin{cases}
2x-4y+\phantom{2}z-w-2t&=0 \\
\phantom{2}x-2y-2z+w&=0 \\
3x-6y-\phantom{2}z\phantom{-w_{2}}-2t&=0
\end{cases}$$
Per poter conoscere $dim \ Sol(SO)$ prima bisogna risolverlo, per farlo useremo l’ eliminazione Gaussiana, come prima cosa leviamo $-\frac{1}{2}*I \ riga$ alla seconda riga:
$$\begin{cases}
2x-4y+\phantom{\frac{5}{2}}z-\phantom{\frac{3}{2}}w-2t&=0 \\
\phantom{2x-2y}-\frac{5}{2}z+\frac{3}{2}w+\phantom{1}t&=0 \\
3x-6y-\phantom{\frac{5}{2}}z\phantom{---}-2t&=0
\end{cases}$$
Come seconda cosa leviamo $-\frac{3}{2} * I \ riga$ alla terza riga:
$$\begin{cases}
2x-4y+\phantom{\frac{5}{2}}z-\phantom{\frac{3}{2}}w-2t&=0 \\
\phantom{2x-2y}-\frac{5}{2}z+\frac{3}{2}w+\phantom{1}t&=0 \\
\phantom{2x-2y}-\frac{5}{2}z+\frac{3}{2}w+\phantom{1}t&=0
\end{cases}$$
Essendo ora la 2° e la terza riga identiche, possiamo sottrarre la 3° riga alla seconda ed avremo risolto il sistema.
$$\begin{cases}
2x-4y+\phantom{\frac{5}{2}}z-\phantom{\frac{3}{2}}w-2t&=0 \\
\phantom{2x-2y}-\frac{5}{2}z+\frac{3}{2}w+\phantom{1}t&=0 \\
\phantom{2x-2y-\frac{5}{2}z+\frac{3}{2}w+3}0&=0
\end{cases}$$
Ora bisogna prestare <font color="#f79646">moltissima</font> attenzione