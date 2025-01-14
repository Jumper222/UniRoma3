---
tags: geometria_e_combinatoria
---
Il nostro primo obiettivo è trovare un <font color="#ffff00">criterio</font> per stabilire se un dato endomorfismo possa essere diagonalizzabile o no.

Se troviamo che sia diagonalizzabile allora descriviamo il procedimento per farlo.

---

Facciamo un esempio, così da avere il criterio ed il procedimento in atto.

Sia $f:R^4[x]\to R^4[x]$ l’ endomorfismo che associa al polinomio $a_{0}+a_{1}x+a_{2}x^2+a_{3}x^3$ al polinomio 
$$(a_{0}+a_{1})+(a_{1}-a_{2}+a_{3})x+(a_{0}+2a_{1}-a_{2})x^2+3a_{3}x^3$$
Consideriamo quindi la base canonica di $R^4$ per la matrice rappresentativa.

<font color="#ffff00">Allora</font> calcoliamo le radici del pol. caratteristico $p_{f}(x):=\det(A-xI)$
Troviamo allora gli autovalori $0$ ed $1$.

Entrambi gli autospazi hanno $dim=1$.

<font color="#4bacc6">Quindi</font> ci possiamo chiedere se $f$ è diagonalizzabile,
Ovvero se esiste una base per $R^4[x]$ formata dagli autovettori di $f$.

Dato che $dim\ E(0)=1$ e $dim\ E(1)=1$, è impossibile che tutti e 4 i polinomi
che formano la base canonica di $R^4$ possano diventare autovettori.

<font color="#f79646">Allora</font> $f$ non è diagonalizzabile.

---

enunciamo quindi qualche teorema legato alla diagonalizzazione:
> [!Enunciato]
> Sia $f:V\to V$ un’ endomorfismo di uno spazio vett. $V$ di dim. finita $n$ e siano $1,2,\dots,s$ gli autovalori distinti di $f$. 
> Se $dim\ E(1)+dim\ E(2)+\dots+dim\ E(s)<n$ allora $f$ <font color="#c0504d">non</font> è diagonalizzabile