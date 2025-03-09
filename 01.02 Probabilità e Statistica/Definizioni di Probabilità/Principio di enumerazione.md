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
$|E|=6*5+5*6=60$
$\mathbb{P}(E)=\frac{60}{110}$, questa è una [[Disposizioni Semplici|disposizione semplice]]

--- 
Un altro esempio potrebbe essere:
$c_{1},\dots,c_{29}$ sono i partecipanti al festival di Sanremo
Allora vi saranno $29!$ classifiche finali possibili.

In generale possiamo dire che ci sono $n!$ modi di ordinare $n$ oggetti distinti.


Allora adesso cerchiamo di sapere quanti sono gli esiti possibili per la top 5, quindi conterà l’ ordine:
Vi saranno $29*28*27*26*25$ esiti possibili, rispettivamente per la 1°,2°,3°,4°,5° scelta

Generalmente quindi ci sono $D_{n,k}=\frac{n!}{(n-k)!}$ modi di disporre una classifica di $k$ oggetti da un gruppo di $n$.


Allora ora ci chiediamo quanti sono gli esiti possibili per la 