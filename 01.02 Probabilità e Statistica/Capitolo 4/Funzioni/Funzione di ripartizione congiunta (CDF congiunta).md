#Probabilità_e_statistica 
>[!Definizione]  Definizione
>La CDF congiunta è un particolare tipo di [[Fun. di Ripartizione (CDF)|CDF]] che come [[Funzioni|funzione]] è tale che:
>$$F_{x,y}:\mathbb{R}_{x}\times\mathbb{R}_{y}\to[0,1]$$
>con
>$$(x,y)\to\mathbb{P}(X\leq x, Y\leq y)$$
>(In questo caso la virgola descrive l’ intersezione dei due eventi!)

Ovviamente essendo che la CDF congiunta di X e Y è creata appunto da X e Y, è possibile ottenere le CDF di X e Y indipendentemente:

Allora chiamiamo:
- $F_{x,y}$ la CDF congiunta
- $F_{x}$ la CDF (<font color="#ffc000">marginale</font>) di X
- $F_{y}$ la CDF (<font color="#ffc000">marginale</font>) di Y

<font color="#f79646">NB</font>: Un discorso analogo vale per la PMF congiunta

Facciamo un esempio:

Consideriamo 2 fabbriche che producono un certo prodotto
Ciascun prodotto può avere 0,1,2 o 3 difetti
Campioniamo un prodotto a caso e chiamiamo:
$X$: $\#$ della fabbrica che lo ha prodotto ($\mathrm{Im}(X)=\{1,2\}$)
$Y$: $\#$ di difetti del prodotto ($\mathrm{Im}(Y)=\{0,1,2,3\}$)
Possiamo specificare la PMF congiunta di X e Y in forma tabellone

![[Esercizio CDF congiunta.png]]

Allora qual’è la probabilità che il prodotto venga dalla seconda fabbrica?
basta semplicemente sommare gli elementi della seconda riga:
$$P_{x}(2)=P_{x,y}(2,0)+P_{x,y}(2,1)+P_{x,y}(2,2)+P_{x,y}(2,3)$$
$$\frac{1}{16}+\frac{1}{16}+\frac{1}{8}+\frac{1}{4}=\frac{1}{12}$$
![[Esempio CDF congiunta 2.png]]
*Possiamo generalizzare dicendo che le marginali si ottengono sommando su righe e colonne*

