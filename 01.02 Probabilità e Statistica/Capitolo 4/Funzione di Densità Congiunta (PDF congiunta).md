#Probabilità_e_statistica 
>[!Definizione]  Definizione
>Chiamiamo Funzione di densità congiunta (PDF congiunta) è una [[Funzioni|funzione]] che prende in input due [[Variabili Aleatorie|v.a.]] [[Variabili Aleatorie discrete e continue|continue]] e restituisce la funzione:
>$$f_{x,y}:\mathbb{R}\times\mathbb{R}\to[0,\infty)$$
>tale che:
>$$F_{X,Y}(x,y)=\int^x_{-\infty}\int^y_{-\infty}f_{X,Y}(u,v)\quad du,dv$$

Esattamente come per la CDF congiunta, è possibile ottenere le PDF marginali a partire dalla congiunta

Qui però andiamo a lavorare con gli integrali doppi:
$\mathbb{P}(X\in[a,b])=\mathbb{P}(X\in[a,b],Y\in\mathbb{R})$
ossia
$$\int^b_{a}\underbrace{\int ^\infty_{-\infty}f_{X,Y}(x,y)dy}_{=f_X(x)}\ dx $$
e analogamente:
$$F_{Y}(y)=\int^\infty_{-\infty}f_{X,Y}(x,y)dx$$

Facciamo un esempio per poter capire meglio:
Siano $X,Y$ v.a. con [[Funzione di ripartizione congiunta (CDF congiunta)|CDF congiunta]]:
$f_{X,Y}$