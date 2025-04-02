Per due variabili aleatorie discrete $X$ e $Y$, la **funzione di massa di probabilità congiunta (o PMF congiunta)** è definita come:

$P_{X,Y}(x,y) = P(X=x, Y=y)$

dove $x$ appartiene all'insieme dei valori possibili di $X$ ($Im(X)$) e $y$ appartiene all'insieme dei valori possibili di $Y$ ($Im(Y)$). Questa funzione associa a ogni coppia di valori $(x, y)$ la probabilità che $X$ assuma il valore $x$ e contemporaneamente $Y$ assuma il valore $y$.

La PMF congiunta può essere rappresentata in forma tabellare, dove le righe e le colonne corrispondono ai possibili valori di $X$ e $Y$ rispettivamente, e le celle contengono le probabilità congiunte.

**Per calcolare la PMF congiunta $P_{X,Y}(x,y)$**, è necessario determinare la probabilità dell'intersezione degli eventi ${X=x}$ e ${Y=y}$. Il modo specifico per calcolare questa probabilità dipende dalla natura delle variabili aleatorie $X$ e $Y$ e dalla loro relazione.

Se la PMF congiunta non è direttamente fornita, può essere derivata in base alle informazioni disponibili sull'esperimento aleatorio e sulla definizione delle variabili $X$ e $Y$.

È importante notare che dalle PMF congiunte, è possibile ricavare le **PMF marginali** di $X$ e $Y$:

- Per la variabile $X$: $P_X(x) = P(X=x) = \sum_{y \in Im(Y)} P(X=x, Y=y) = \sum_{y \in Im(Y)} P_{X,Y}(x,y)$
- Per la variabile $Y$: $P_Y(y) = P(Y=y) = \sum_{x \in Im(X)} P(X=x, Y=y) = \sum_{x \in Im(X)} P_{X,Y}(x,y)$

In pratica, se si ha una tabella che rappresenta la PMF congiunta, le PMF marginali si ottengono sommando i valori rispettivamente per riga (per $Y$) o per colonna (per $X$).

Ad esempio, considerando due fabbriche che producono un certo prodotto con un numero variabile di difetti, se $X$ è la variabile che indica la fabbrica (con valori 1 o 2) e $Y$ è la variabile che indica il numero di difetti (con valori 0, 1, 2, 3), la PMF congiunta $P_{X,Y}(x,y)$ fornisce la probabilità che un prodotto provenga dalla fabbrica $x$ e abbia $y$ difetti. Per trovare la probabilità che un prodotto provenga dalla seconda fabbrica ($P_X(2)$), si sommano tutte le probabilità congiunte in cui $X=2$.