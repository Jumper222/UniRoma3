---
tags:
  - Probabilità_e_statistica
aliases:
  - PDF Congiunta
  - PDF congiunta
---

>[!Definizione]  Definizione
>Chiamiamo Funzione di densità congiunta ([[Fun. di densità di Probabilità (PDF)|PDF]] congiunta) è una [[Funzioni|funzione]] che prende in input due [[Variabili Aleatorie|v.a.]] [[Variabili Aleatorie discrete e continue|continue]] e restituisce la funzione:
>$$f_{x,y}:\mathbb{R}\times\mathbb{R}\to[0,\infty)$$
>tale che:
>$$F_{X,Y}(x,y)=\int^x_{-\infty}\int^y_{-\infty}f_{X,Y}(u,v)\quad du,dv$$

Esattamente come per la [[Funzione di ripartizione congiunta (CDF congiunta)|CDF congiunta]], è possibile ottenere le [[Fun. di densità di Probabilità (PDF)|PDF]] marginali a partire dalla congiunta

Qui però andiamo a lavorare con gli integrali doppi:
$\mathbb{P}(X\in[a,b])=\mathbb{P}(X\in[a,b],Y\in\mathbb{R})$
ossia
$$\int^b_{a}\underbrace{\int ^\infty_{-\infty}f_{X,Y}(x,y)dy}_{=f_X(x)}\ dx $$
e analogamente:
$$F_{Y}(y)=\int^\infty_{-\infty}f_{X,Y}(x,y)dx$$

Facciamo un esempio per poter capire meglio:
Siano $X,Y$ [[Variabili Aleatorie|v.a.]] con [[Funzione di ripartizione congiunta (CDF congiunta)|CDF congiunta]]:
$$f_{X,Y}(x,y)=\begin{cases}
2e^{-x}e^{-2y} & \text{se }x>0\ e \ y>0 \\
0 & altrimenti
\end{cases}$$
![[01.02 Probabilità e Statistica/Immagini/PDF congiunta esempio.png]]

Ora ci chiediamo quanto vale $\mathbb{P}(X>1,Y<1)?$
$$\mathbb{P}(X>1,Y<1)=\int^1_{0}\int^\infty_{1}2e^{-x}e^{-2y}dx\ dy$$
$$=\int_{0}^12e^{-2y}\left( \int_{1}^\infty e^{-x}dx \right)dy$$
$$=\int_{0}^12e^{-2y}(-e^{-x})|^\infty_{1}dy$$
$$=\int_{0}^12e^{-2y}\ e^{-1}dy$$
$$=2e^{-1}\int_{0}^1e^{-2y}dy$$
$$=2e^{-1}\left( -\frac{1}{2}e^{-2y} \right)^1_{0}$$
$$=2e^{-1}\left( -\frac{1}{2}e^{-2}+\frac{1}{2} \right)$$
$$=e^{-1}(1-e^{-2})\approx 0,318$$
![[Esempio PDF congiunta.png]]
![[PDF congiunta esempio 1.png]]