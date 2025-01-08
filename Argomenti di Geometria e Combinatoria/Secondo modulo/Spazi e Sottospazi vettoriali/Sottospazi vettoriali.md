I <font color="#ffff00">sottospazi vettoriali</font>, come dice il nome sono i sottoinsiemi di uno<font color="#76923c"> spazio vettoriale</font>, con essi stessi definibili come spazi vettoriali.

Innanzitutto, un sottoinsieme di uno spazio vettoriale non è per forza un <font color="#ffff00">sottospazio vettoriale</font>.

Prendiamo in esame il sottoinsieme $E$ di $M(2,2,\mathbb{R})$.
Questo sottoinsieme è definito con tutte le matrici 2x2 che hanno almeno un elemento nullo.
Allora prendiamo 2 elementi $A,B\in E$ 
$$A:=\begin{pmatrix}1 & -2 \\0 & 2\end{pmatrix} , \quad B:=\begin{pmatrix}0&1\\3 & 2\end{pmatrix}$$
Da una rapida verifica possiamo notare che la proprietà dell’ addizione degli <font color="#76923c">spazi vettoriali</font> <font color="#d83931">non</font> è verificata
(La proprietà dice che $A+B$ dovrebbe essere una operazione che restituisce un valore all’ interno dello <font color="#76923c">spazio vettoriale</font>, in questo caso la nuova matrice si trova fuori da $E$.)

Infatti abbiamo che: $$A+B=\begin{pmatrix}1 & -2 \\0 & 2\end{pmatrix}+ \begin{pmatrix}0&1\\3 & 2\end{pmatrix} =\begin{pmatrix}1&-1\\3&4\end{pmatrix}$$
Che non è una matrice che appartiene ad $E$.

Volessimo quindi dare una definizione di <font color="#ffff00">sottospazio vettoriale</font> sarebbe la seguente:

- Un <font color="#ffff00">sottospazio vettoriale</font> $E$ può essere considerato tale se rispetta tutte le proprietà di uno <font color="#9bbb59">spazio vettoriale</font>, con particolare attenzione alle seguenti:
  - $u+v\in E \ \ \forall u,v\in E$
  - $ku\in E \ \ \forall u\in E, \ \ \forall k\in\mathbb{R}$
  - $u+0=u, \\ \forall u,0\in E$ (Esistenza dell’ elemento neutro nell’ addizione)
  - $u+(-u)=0, \\ \forall u,-u\in E$ (Esistenza dell’ opposto)

Data la definizione di un sottospazio vettoriale, possiamo [[Esempi di sottospazi vettoriali|Elencarne]] alcuni molto usati

Un tipo molto particolare  di sottospazio vettoriale è il [[Sottospazi Affini|Sottospazio Affine]]

I sottospazi vettoriali hanno delle [[Dimensioni]]