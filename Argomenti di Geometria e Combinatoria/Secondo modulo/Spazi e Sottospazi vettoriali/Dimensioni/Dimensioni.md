La dimensione di uno spazio vettoriale è il numero di vettori contenuti nella base dello spazio:

Dato uno spazio con al suo interno 3 punti: $A,B,C$ non complanari tra loro, allora i vettori $v_{1}:=\overrightarrow{OA},v_{2}:=\overrightarrow{OB},v_{3}:=\overrightarrow{OC}$ sono linearmente indipendenti quindi ogni vettore all’ interno dello spazio è descritto da $v_{1},v_{2},v_{3}$, che essendo 3 vettori allora lo spazio ha dimensione 3.

La notazione che usiamo per descrivere la dimensione di uno spazio vettoriale:

$$dim \ V^2(O)=2$$

Se uno <font color="#4bacc6">spazio vettoriale</font> ha una base formata da $n$ vettori (Cioè dim $V=n$) allora si dice che $V$ ha una <font color="#ffff00">dimensione finita</font>

Se invece uno spazio vettoriale non può essere descritto da una base (non è finitamente generato) allora si dice che ha una <font color="#ffff00">dimensione infinita</font>.

è utile anche ricordare alcune delle <font color="#ffff00">dimensioni</font> degli spazi vettoriali più comuni
- $dim \ V^2(O)=2$
- $dim \ V^3(O)=3$
- $dim \ \mathbb{R}^n=n$
- $dim \ M(p,q,R)=p*q$
- $dim \ \mathbb{R}^n[x]=n$


### <font color="#4bacc6">Osservazioni utili sulle dimensioni</font>

Se $dim \ V=n$ allora:
- Non esistono più di $n$ vettori linearmente indipendenti
- Dati comunque $r$ vettori con $r<n$ (anche se linearmente indipendenti), essi non possono essere generatori (e quindi tantomeno una base) di $V$
- Dati comunque $n$ vettori linearmente indipendenti, essi costituiscono una base di $V$
- Dati comunque $n$ generatori, essi formano una base di $V$

Dunque, se volessimo controllare se dati $n$ vettori di uno spazio $v$ essi formano una base allora possiamo controllare:
- Che gli $n$ vettori siano generatori,
- Oppure che gli $n$ vettori siano linearmente indipendenti


Potrebbe essere utile anche studiare 2 semplici esempi per comprendere meglio come trovare la dimensione di uno spazio vettoriale
### <font color="#4bacc6">Esempio 1</font>

Dati i seguenti vettori appartenenti a $\mathbb{R}^3$: $$v_{1}:=(1,2,1),v_{2}:=(1,1,1),v_{3}:=(0,1,2),v_{4}:=(1,1,3) $$
Stabilire se sono linearmente indipendenti.

Possiamo subito stabilire che $dim \ \mathbb{R}^3=3$, che impone quindi che possano esistere solo fino a 3 vettori linearmente indipendenti nello stesso momento all’ interno dello spazio, di conseguenza si evince subito essi non possono essere linearmente indipendenti.


### <font color="#4bacc6">Esempio 2</font>

Date le seguenti matrici, stabilire se esse generano $M(2,2,R)$:
$$A_{1}:=\begin{pmatrix}
1&1 \\
0&0
\end{pmatrix}, \quad A_{2}:=\begin{pmatrix}
0&1 \\
1&-1
\end{pmatrix}, \quad A_{3}:=\begin{pmatrix}
0&2 \\
2&0
\end{pmatrix}$$
Sappiamo che $dim \ M(2,2,R)=4$,
Quindi per poter generare questo spazio vettoriale sono necessari come base almeno 4 vettori linearmente indipendenti tra loro.
Avendo noi qui soltanto 3 matrici, ovviamente esse non possono generare $M(2,2,R)$.

Ora andiamo a vedere come si relazionano le [[Dimensioni di sottospazi vettoriali|Dimensione e sottospazi vettoriali]]