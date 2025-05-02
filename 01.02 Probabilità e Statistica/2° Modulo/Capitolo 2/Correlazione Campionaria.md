---
tags:
  - Probabilità_e_statistica
---

>[!Definizione]  Definizione
>Dato un [[Insieme di Dati Bivariati|campione bivariato]], $((x_{1},y_{1}),\dots,(x_{n},y_{n}))$ Il Coefficiente di Correlazione Campionaria è la quantità t.c:
>$$r=\dfrac{ \sum^n_{i=1}(x_{i}-\bar{x})(y_{i}-\bar{y})}{(n-1)S_{x}S_{y}}$$
>Esattamente come la normale [[Correlazione]], quella campionaria esiste tra 0 ed 1, e presenta 3 stati:
>- Due dati si dicono <font color="#ffff00">correlati positivamente</font> se $r>0$
>- Si dicono <font color="#ffff00">non correlati</font> se $r=0$
>- Si dicono <font color="#ffff00">correlati negativamente</font> se $r<0$
> 


Se trasformiamo il campione bivariato $(x_{i},y_{i})$ in $((a+bx_{i}),(c+dy_{i}))$ con $b,d$ aventi lo stesso segno,
Allora il loro coefficiente di correlazione non cambia.

<font color="#4bacc6">Attenzione</font>! La correlazione non implica un rapporto di causa effetto

##### Forza di una correlazione

- Se $|r|=1$ i dati poggiano tutti su una retta
- Se $|r|>0.8$ si ha una <font color="#f79646">correlazione intensa</font>
- Se $|r|<0.5$ si ha una <font color="#f79646">correlazione debole</font>

