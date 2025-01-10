Per <font color="#9bbb59">cambio di base</font> si intende appunto un cambiamento alla base di un <font color="#92d050">endomorfismo</font> che va poi a modificare la matrice rappresentativa.

Ed è definita tale che:

Sia $V$ uno spazio vettoriale di dimensione finita $n$. 
Si considerino ora 2 basi di $V$:

- Una formata dai vettori $e_{1},e_{2},\dots,e_{n}$
- Una seconda formata dai vettori $e'_{1},e'_{2},\dots,e'_{n}$

La matrice $M$ in $M(n,n,R)$ la cui $j$-esima colonna è data dalle componenti del vettore $e'_{j}$ rispetto la base formata dai vettori $e_{1},e_{2},\dots,e_{n}$. Questa matrice è detta <font color="#f79646">matrice di passaggio</font> dalla base formata da $e_{1},e_{2},\dots ,e_{n}$ alla base formata da $e'_{1},e'_{2},\dots,e'_{n}$

---

Facciamo un semplicissimo esempio:

Consideriamo $R^3[x]$:

Vogliamo effettuare il <font color="#ffff00">cambio di base</font> tra la sua base canonica:
- $q_{1}(x):=1$
- $q_{2}(x):=x$
- $q_{3}(x):=x^2$
ed una seconda <font color="#ffff00">base</font> formata da:
- $p_{1}(x):=(1,x,x^2)$
- $p_{2}(x):=(1,x)$
- $p_{3}(x):=(1)$

Il nostro obiettivo sarà quello di trovare la matrice $M$ di passaggio tra la prima e la seconda base, <font color="#f79646">dovremo quindi</font> esprimere $p_{1},p_{2},p_{3}$ come comb. lineari di $q_{1},q_{2},q_{3}$:

- $p_{1}(x)=1q_{1}(x)+1q_{2}(x)+1q_{3}(x)$
- $p_{2}(x)=1q_{1}(x)+q_{2}(x)$
- $p_{3}(x)=1q_{1}(x)$

Ed allora la matrice rappresentativa risulterà:

$$M:=\begin{pmatrix}
1 & 1 & 1 \\
1 & 1 & 0 \\
1 & 0 & 0
\end{pmatrix}$$

<font color="#f79646">NB</font>: La matrice di passaggio sarà sempre invertibile, e ci viene in aiuto il seguente [[Teorema sull’ invertibilità della matrice di passaggio|teorema]]


---

Se si volesse rieffettuare il cambio dalla seconda base alla prima, sapremo che la nuova matrice rappresentativa sarà $M^{-1}$, ossia la matrice inversa. Per ottenere questa matrice ci basterà esprimere i vettori della prima base come comb. lineare dei vettori della seconda.

---

Se si volesse calcolare un endomorfismo in un’ altra base:

Data una matrice $A$, rappresentativa di $f$ nella base iniziale
Data una matrice $M$, la matrice di passaggio dalla prima alla seconda base

Allora avremo la matrice $A'$, rappresentativa di $f$ nella seconda base tale che:
$$A'=M^{-1}A\ M$$

---

Un altro utile concetto è che se le matrici $A,B$ rappresentano lo stesso endomorfismo rispetto basi diverse,

Allora esisterà una matrice invertibile $M$ tale che $B=M^{-1}A\ M$

E quindi nasce il concetto di [[Matrici Simili|matrici simili]].