Dato un omomorfismo $f:V\to W$, e fissata una base per $V,W$
Sia $A$ la matrice rappresentativa di $f$ rispetto tali basi.
Allora avremo $dim\ ker\ f=dim\ V-rk\ A$

---

Sia $f:V\to W$ un omomorfismo, se $V$ ha dimensione <font color="#ffff00">finita</font>, risulterà $dim\ (V)=dim\ ker \ f+dim\ f(V)$

---

Se l’omomorfismo $f$ è iniettivo, allora $dim\ V=dim\ f(V)$ ed avremo che poiché $f(V)$ è un sottospazio di $W$, segue che $dim\ V\leq dim\ W$ 

<font color="#ff0000">NB</font>: se $dim\ V>dim\ W$ allora $f$ non può essere iniettivo.

--- 

Possiamo quindi dare per equivalenti le seguenti definizioni:
- $f$ è iniettivo
- $rk\ A=dim\ V$
- $dim\ f(V)=dim\ V$.


Alcuni stupidi esempi potrebbero essere:
- $f:R[x]\to R^3$, non è iniettivo perché va da un insieme infinito ad uno finito
- $f:M(2,2,R)\to R^3$, non è iniettivo perché $dim\ M(2,2,R)>dim\ R^3$

Non possiamo però escludere a priori che $R^3\to M(2,2,R)$ non sia iniettivo, esplichiamolo:

$$f(a,b,c):=\begin{pmatrix}
a-4b & b-2c \\
a+3c & a+b+c
\end{pmatrix}$$
Quindi usiamo la matrice rappresentativa $A$ rispetto le basi canoniche:
$$A:=\begin{pmatrix}
1 & -4 & 0 \\
0 & 1 & -2 \\
1 & 0 & 3 \\
1 & 1 & 1
\end{pmatrix}$$
Possiamo calcolare che essa ha $rk=3$ quindi $rk\ A=dim\ V$, quindi  $f$ è iniettivo