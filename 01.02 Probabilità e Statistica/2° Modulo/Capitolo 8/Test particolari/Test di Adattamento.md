---
tags:
  - Probabilità_e_statistica
---
Facciamo un esempio:

![[Test di Adattamento ESEMPIO.png]]

Abbiamo un campione $Y_{1}\dots Y_{n}\in\{-6,-5\dots5\}$ *12 categorie*

Chiamo $X_{-6}\dots X_{5}$ quante $Y$ valgono $i$:
$$X_{i}=\sum^n_{j=1}\mathbb{1}(Y_{j}=i)$$

Allora per testare l’ affermazione qui sopra creo le ipotesi:
$H_{0}:\mathbb{P}(Y=i)=\dfrac{1}{12}$
$H_{1}:\mathbb{P}(Y=i)\neq \dfrac{1}{12}$
*Per un qualche $i$ compreso tra -6 e 5*

Allora per individuare la [[Statistica Test]] uso la formula:

$$\left(\sum^k_{i=1} \dfrac{x_{i}^2}{np_{i}}\right)-n$$
- $x^2_{i}$ è il numero di osservazioni nella categoria $i$, portato al quadrato.
- $np_{i}$ è il [[Valore Atteso]] per quella categoria, in questo caso $\dfrac{n}{12}$ dove $n$ è il numero di osservazioni in quella categoria, e $\dfrac{1}{12}$ è la grandezza di quella categoria.


Se $H_{0}$ è vera ed $n\gg 1$, allora $T\sim \chi^2_{11}$ *La dimostrazione verrà saltata a piè pari*
Allora fissato un [[Livello di Significatività]] $\alpha$:
- Se $T\leq \chi^2_{\alpha,11}$ Non rifiuto $H_{0}$
- Se $T>\chi^2_{11}$ Rifiuto $H_{0}$

Nota: I gradi di liberta della $\chi^2$ sono k-1.

La [[p-value]] invece si calcola:
$\mathbb{P}(\chi^2_{k-1}>st)$ *Dove k è il numero di categorie*
