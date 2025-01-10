Sappiamo già che gli <font color="#9bbb59">autovalori</font> servono per diagonalizzare una matrice, e che si indicano con $\lambda$.
Studiamo un esempio e poi andiamo a definirli meglio.

---

Sia dato l’ endomorfismo di $R^3$, definito da $f(x,y,z):=(2x+2y+z,y,0)$
Stabiliamo per ciascuno di questi vettori se è sono <font color="#4bacc6">autovettori</font> di $f$.
in caso affermativo determinare l’ <font color="#4bacc6">autovettore</font> corrispondente:

- $v_{1}:=(1,0,0)\to f(v_{1})=f(1,0,0)=(2,0,0)$ <font color="#ffff00">OK!</font> $\to f(v_{1})=2v_{1}$
- $v_{2}:=(0,1,0)\to f(v_{2})=f(0,1,0)=(2,1,0)$ <font color="#ff0000">NO!</font>, non è multiplo di $v_{2}$.
- $v_{3}:=(1,0,-2)\to f(v_{3})=f(1,0,-2)=(0,0,0)$ <font color="#ffff00">OK!</font> $\to f(v_{3})=0(v_{3})$
- $v_{4}:=(0,0,0)$ <font color="#ff0000">non</font> è un autovettore in quanto per definizione essi sono diversi dal vettore nullo.

---

Vediamo ora cosa è un’ autospazio:

<font color="#f79646">Teorema</font>: Sia $f:V\to V$ un endomorfismo di uno spazio vettoriale $V$ e sia $\lambda$ un <font color="#9bbb59">autovalore</font> di $f$. L’ insieme $$E(\lambda):=\{v\in V\ |\ f(v)=\lambda(v) \}$$
è un <font color="#ffff00">sottospazio vettoriale</font> di $V$, detto <font color="#92cddc">autospazio</font> di $f$ relativo a $\lambda$. 

<font color="#f79646">Def</font>: $E(\lambda)$ è formato dagli <font color="#4bacc6">autovettori</font> di $f$ relativi all’ autovalore $\lambda$ e dal vettore nullo.
(Per definizione di <font color="#4bacc6">autovettore</font> $v\neq 0$, un <font color="#92cddc">autospazio</font> non può mai essere formato dal solo vettore nullo)

<font color="#f79646">Dimostrazione</font>: $E(\lambda)$ è non vuoto perché contiene il vettore nullo.
se $v_{1},v_{2}$ sono vettori di $E(\lambda)$ allora anche $v_{1}+v_{2}\in E(\lambda)$? 

Sappiamo che $f(v_{1})=\lambda v_{1},f_{2}=\lambda v_{2}$ e dobbiamo mostrare che $f(v_{1}+v_{2})=f(v_{1})+f(v_{2})=\lambda v_{1}+\lambda v_{2}=\lambda(v_{1}+v_{2})$

Ora che sappiamo che rispetta l’ addizione, controlliamo la moltiplicazione:

