#Probabilità_e_statistica 
>[!Definizione]  Definizione
>Due eventi si dicono indipendenti quando l’ avvenimento di uno non condiziona l’ altro
>$$\mathbb{P}(E|F)=\mathbb{P}(E)$$
>Allora gli eventi si scrivono $E\coprod F$ ossia indipendenti tra loro $\mathbb{P}(E\cap F)=\mathbb{P}(E)\mathbb{P}(F)$

Inoltre abbiamo la relazione:
$$E\coprod F\implies E \coprod F^c$$
Inoltre se 3 eventi sono <font color="#f79646">indipendenti</font> tra loro allora ognuno è indipendente dalle unioni/intersezioni degli altri 2.

Allora generalmente diciamo che $E_{1},\dots,E_{k}$ sono indipendenti se:
$\mathbb{P}\left( \bigcap_{i\in I} \right)=\prod_{i\in I}\mathbb{P}(E_{i}), \quad \quad \forall I\subset\{1,\dots,k\}$


Facciamo un esempio:
Estraggo una carta a caso da un mazzo francese
- $A$:”esce un asso”
- $C$:”esce una carta di cuori”

Allora avremo $\mathbb{P}(A)=\frac{4}{52}=\frac{1}{13}$
E inoltre $\mathbb{P}(C)=\frac{13}{52}=\frac{1}{4}$
Quindi $\mathbb{P}(A\cap C)=\frac{1}{13}* \frac{1}{4}\implies A \coprod C$

Ora facciamo un altro esempio:

Ho un circuito in parallelo, con $n$ resistenze, con la condizione che il circuito funziona se almeno una componente funziona

Quindi supponiamo di sapere che la componente i-esima funziona con prob. $p_{i}$ indipendente dalle altre.
$A_{1}$= “L’ iesima funziona”
$F$ = “Il circuito funziona”

$\mathbb{P}(F)=1-\mathbb{P}(F^c)$
Quindi se $p_{i}=p$