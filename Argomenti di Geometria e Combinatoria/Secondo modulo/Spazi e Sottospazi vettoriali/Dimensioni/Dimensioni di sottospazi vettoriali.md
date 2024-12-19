Diamo alcune utili osservazioni riguardo le dimensioni dei sottospazi vettoriali

- Sia $V$ uno spazio vettoriale di dimensione finita, con al suo interno il <font color="#ffff00">sottospazio</font> vettoriale $E$ 
  Allora $E$ ha dimensione finita e $dim \ E\leq dim \ V$

- Sia $V$ uno spazio vettoriale e $dim \ V=n$, allora:
  - Esiste un <font color="#ffff00">sottospazio</font> $E$ con $dim \ E=0$, formato dal vettore nullo.
  - Esiste un <font color="#ffff00">sottospazio</font> di $dim$ uguale ad $n$, formato da $V$ stesso.

Un esempio di queste proprietà sarebbe il seguente:

- Prendiamo lo spazio vettoriale $V^2(O)$ ha $dim=2$
  - Possiamo quindi dire che i suoi <font color="#ffff00">sottospazi</font> possono avere $dim=1 \ oppure\ 2$
  - L’unico <font color="#ffff00">sottospazio</font> di $dim=0$ consiste nel vettore nullo.
  - I <font color="#ffff00">sottospazi</font> di $dim=1$ sono quelli di tipo $\{\overrightarrow{OP}\ |P\in r\}$
  - L’unico <font color="#ffff00">sottospazio</font> di $dim=2$ è $V^2(O)$

Facciamo ora qualche esempio:

### <font color="#4bacc6">Esempio 1</font>

Definiamo $S(2,R)$ come sottospazio vettoriale all’ interno di $M(2,2,R)$ composto dalle sole matrici simmetriche. vogliamo ora determinarne una base.

- Procederemo per step, andando ad aumentare volta in volta le dimensioni dello spazio che stiamo studiando.
- Innanzitutto prendiamo in considerazione il sottospazio vettoriale $V_{1},$ con base $S_{1}$ definita tc:
$$S_{1}:=\begin{pmatrix}
0 & 1 \\
1& 0
\end{pmatrix}$$
- Possiamo subito notare che $V_{1}$ non può costituire la base di $S(2,R)$ perché ci sarebbero alcune matrici non all’ interno di $V_{1}$ ma all’ interno di $S(2,R)$, come $S_{2}$:
$$S_{2}:=\begin{pmatrix}
1&0 \\
0&0
\end{pmatrix}$$
- Allora studiamo il sottospazio di $S(2,R)$: $V_{2}$, con base $S_{1},S_{2}$:
$$V_{2}=\begin{pmatrix}
a&b \\
b&0
\end{pmatrix}$$
- Anche in questo caso purtroppo non riusciamo ancora a descrivere l’ intero sottospazio vettoriale $S(2,R)$, in quanto abbiamo $S_{3}$ non descritta:
$$S_{3}:=\begin{pmatrix}
0&0 \\
0&1
\end{pmatrix}$$
- Ed allora espandiamo ancora lo spazio vettoriale studiato, analizzando $V_{3}$ con base $S_{1},S_{2},S_{3}$:
 $$V_{3}=\begin{pmatrix}
a&b \\
b&c
\end{pmatrix}$$
- Possiamo finalmente dire che questo sottospazio coincide con $S(2,R)$. Questo sottospazio vettoriale avrà quindi $dim=3$ perché è descrivibile dalla base canonica $S_{1},S_{2},S_{3}$.

