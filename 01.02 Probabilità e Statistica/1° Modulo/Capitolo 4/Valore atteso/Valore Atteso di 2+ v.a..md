#Probabilità_e_statistica 
Potrebbe capitarci di dover ottenere il [[Valore Atteso]] di due o più [[Variabili Aleatorie]] 
Allora mostriamo il processo per calcolare il [[Valore Atteso]] per due va. continue:

Siano $X$ e $Y$ sono due [[Variabili Aleatorie discrete e continue|v.a. continue]], e $g:\mathrm{Im}(X)\times \mathrm{Im}(Y)\to\mathbb{R}$
allora $g(x,y)$
Allora il v.a. sarà:
$$\mathbb{E}[g(X,Y)]=\int^\infty_{-\infty}\int^\infty_{-\infty}g(x,y)f_{X,Y}(x,y)dx\ dy$$
E si ha un meccanismo analogo per $X,Y$ discrete:

Facciamo un esempio:
$g(x,y)=x+y$
![[Valore Atteso di 2+ v.a..png]]

E allora il [[Valore Atteso]] della somma di due v.a. è la somma dei valori attesi delle v.a.

Questo concetto si estende anche a più di 2 v.a. nello stesso modo. 