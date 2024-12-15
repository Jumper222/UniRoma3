### <font color="#4bacc6">Esempio 1 di un generatore</font>

- Abbiamo l’ insieme $L(v_{1},v_{2},\dots v_{r})$
  Notiamo subito che $L$ contiene tutti i vettori $v_{1},v_{2},\dots v_{r}$
  Ad <font color="#ffff00">esempio</font> $v_{1}=1v_{1}+0v_{2}+\dots+0v_{r}$
  Allora definiamo $E$ come un sottospazio vettoriale di $V$ contenente $v_{1},v_{2},\dots v_{r}$
  Allora per definizione di un sottospazio vettoriale possiamo anche dire che $E$ contiene anche               tutti i vettori del tipo $k_{1}v_{1},k_{2}v_{2},\dots,k_{r},v_{r}$
  Allora di conseguenza $E$ contiene anche tutte le combinazioni lineari del tipo $k_{1}v_{1}+k_{2}v_{2}+\dots+k_{r}v_{r}$
  **<font color="#f79646">QUINDI</font> possiamo dire che $E$ è generato da $L(v_{1},v_{2},\dots, v_{r})$

  In altre parole, essendo $E = L(v_{1},v_{2},\dots,v_{r})$ allora $E$ è <font color="#ffff00">generato</font> dai vettori $v_{1},v_{2},\dots,v_{r}$
  E quindi abbiamo anche il rapporto inverso:
  $v_{1},v_{2},\dots, v_{r}$ sono generatori di $E$ (dato se e solo se ogni vettori di $E$ è comb. lineare di $v_{1},v_{2},\dots,v_{r}$ )

### <font color="#4bacc6">Esempio 2 di un generatore</font>

- Data una retta $r$ passante per l’ origine $O$ del piano, e dato un punto $A$ della retta $r$ distinto da $O$,
  l’insieme dei <font color="#e36c09">vettori</font> $\overrightarrow{OP}$ con $P$ giacente su $r$ è un sottospazio vettoriale <font color="#ffff00">generato</font> dal vettore $\overrightarrow{OA}$
  Possiamo quindi dire che dati in $V^2(O)$ due <font color="#e36c09">vettori</font> $\overrightarrow{OP}_{1}$ e $\overrightarrow{OP}_{2}$ con $O$, $P_{1}$ e $P_{2}$ non allineati, i <font color="#e36c09">vettori</font> $\overrightarrow{OP}_{1}$ e $\overrightarrow{OP}_{2}$ <font color="#ffff00">generano</font> $V^2(O)$.

### <font color="#4bacc6">Esempio 3 di un generatore</font>

- Consideriamo le seguenti tre matrici di $M(2,2,\mathbb{R})$
  $A_{1}:=\begin{pmatrix}1&2\\2&0\end{pmatrix}, \quad A_{2}:=\begin{pmatrix}3 &1\\1 &0\end{pmatrix}, \quad A_{3}:=\begin{pmatrix}0&2\\2&0\end{pmatrix}$
  Allora il sottospazio vettoriale che esse <font color="#ffff00">generano</font> è formato dalle matrici del tipo $k_{1}A_{1}+k_{2}A_{2}+K_{3}A_{3}$ infatti:
  $$\begin{pmatrix}k_{1}+3k_{2} &2k_{1}+k_{2}+2k_{3}\\2k_{1}+k_{2}+2k_{3} &0\end{pmatrix}$$
  (I coefficienti sono dati dai numeri all’ interno delle matrici)


### <font color="#4bacc6">Esempio 4 di un generatore</font>
- Consideriamo i tre polinomi $1,x,x^2$.
  Vediamo che le loro combinazioni lineare sono tutti i polinomi del tipo:
  $$k_{1}+k_{2}x+k_{3}x^2$$
  Dunque abbiamo che $1,x,x^2$ <font color="#ffff00">generano</font> $R^3[x]$ ovvero il sottospazio vettoriale di $R[x]$ formato dai polinomi di grado minore di 3.
  - Analogamente si potrebbe verificare che $1,x,x^2,\dots,x^n$ <font color="#ffff00">generano</font> $R^{n+1}[x]$


### <font color="#4bacc6">Esempio 5 di un generatore</font>
- Ora vediamo un’ esercizio che può verosimilmente uscire all’ esame.

- Sia $E$ il sottospazio vettoriale di $R^4$ generato dai vettori:
- $v_{1}:=(3,2,2,1),v_{2}:=(1,0,1,-1) \ e \ v_{3}:=(0,1,1,2)$
- Stabilire se il vettore $v:=(0,1,0,2)\in E$

- Per risolvere l’ esercizio innanzitutto poniamoci la domanda in forma di una combinazione lineare:
- $(0,1,0,2)=k_{1}(3,2,2,1)+k_{2}(1,0,1,-1)+k_{3}(0,1,1,2)$
  Ovvero:
  $(0,1,0,2)=(3k_{1}+k_{2},\ 2k_{1}+k_{3},\ 2k_{1}+k_{2}+k_{3},\ k_{1}-k_{2}+2k_{3})$
  Quindi possiamo andare a risolvere il sistema correlato:
  $$$$