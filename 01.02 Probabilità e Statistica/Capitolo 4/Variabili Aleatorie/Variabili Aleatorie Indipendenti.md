---
tags:
  - Probabilità_e_statistica
aliases:
  - v.a. indipendenti
  - V.a. indipendenti
---

>[!Definizione]  Definizione
>Esattamente come gli [[Eventi indipendenti]], Le [[Variabili Aleatorie|v.a.]] indipendenti sono un particolare tipo di v.a. di cui l’ avvenimento di una non modifica il comportamento dell’ altra.
>Per sapere se due v.a. sono indipendenti calcoliamo:
>$$F_{X,Y}=F_{X}(x)F_{Y}(y)\quad \forall x,y\in\mathbb{R}$$
>O se fossero discrete possiamo anche:
>$$P_{X,Y}(x,y)=P_{X}(x)P_{Y}(y)$$
>ovviamente con x e y che sono immagini di X e Y

Un particolare tipo di v.a. Indipendenti sono le [[IID]]

Facciamo un esempio:

Consideriamo 2 fabbriche che producono un certo prodotto ciascun prodotto può avere 0,1,2,3 difetti,
campioniamo un prodotto a caso e chiediamo:
- $X$: = # della fabbrica che lo ha prodotto ($\mathrm{Im}(X)=\{1,2\}$)
- $Y$: = # di difetti del prodotto ($\mathrm{Im}(Y)=\{0,1,2,3\}$)

Possiamo specificare la PMF congiunta di $X$,$Y$ in forma tabellone:
![[v.a. indipendenti esempio.png]]

Allora consideriamo i due eventi:
- $E=\{X=1\}$
- $F=\{Y=1\}$

Allora calcoliamo:
$$\mathbb{P}(E\cap F)=\mathbb{P}(X=1,Y=1)=\frac{1}{16}$$
e anche
$$\mathbb{P}(E)\mathbb{P}(F)=\mathbb{P}(X=1)\mathbb{P}(Y=1)=\frac{1}{2}* \frac{2}{16}=\frac{1}{16}$$
Visto che la probabilità rimane uguale in questi due casi allora i due eventi sono: $E\coprod F$ indipendenti

Però, se consideriamo gli eventi:
- $E=\{X=1\}$
- $G=\{Y=0\}$

$\mathbb{P}(E\cap G)=\mathbb{P}(X=1,Y=0)=\frac{1}{8}$
ma invece
$\mathbb{P}(E)|\mathbb{P}(G)=\frac{1}{2}* \frac{3}{16}> \frac{1}{8}$
Le due v.a. non sono indipendenti.

