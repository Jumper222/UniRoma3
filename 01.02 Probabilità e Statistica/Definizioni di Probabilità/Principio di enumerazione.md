#Probabilità_e_statistica 
>[!Definizione]  Definizione
>Dati $k\geq 1$ esperimenti,
>
>$n_{1}$ esiti possibili per il 1°
>$n_{2}$ esiti possibili per il 2°
>$n_{k}$ esiti possibili per il k°
>
>Allora possiamo dire il complesso di $K$ esperimenti sarà dato da:
>$$\prod_{i=1}^k n_{i}$$
>Ossia Il prodotto tra tutto il numero di esiti del primo esperimento per il numero di esiti del secondo e cosi via

Per capire meglio facciamo un esempio:

Un urna contiene:
$6$ palle bianche $(1,\dots,6)$
$5$ palle nere $(7,\dots,11)$

Estraggo 2 palle dall’ urna, senza reinserirle
Allora $\Omega$ sarà nella forma
$$\Omega=\begin{pmatrix}
(1,2) & (1,3) & \dots & (1,11) \\
(2,1) & (2,3) & \dots & (2,11) \\
\vdots & \vdots &  & \vdots \\
(11,1) & (11,2) & \dots & (11,10)
\end{pmatrix}$$
Quindi $$|\Omega|=\underbrace{11}_{\text{Scelte per la 1° pallina}}*\underbrace{10}_{\text{scelte per la 2° pallina}}=110$$
Questa è una [[Permutazioni Semplici|permutazione semplice]], che si ha in generale per ogni $|\Omega|$ di uno [[Spazio equiprobabile]]

Allora $E$: Estraggo 1 bianca e 1 nera, non necessariamente in questo ordine
$|E|=6*5+5*6=60$, Questa è una [[Permutazioni Semplici]]
$\mathbb{P}(E)=\frac{60}{110}$
