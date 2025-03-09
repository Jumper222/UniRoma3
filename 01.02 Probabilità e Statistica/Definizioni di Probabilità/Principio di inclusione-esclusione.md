#Probabilità_e_statistica 
la principale raison d’être <font color="#ffff00">principio di inclusione/esclusione</font> è di non contare doppiamente l’ eventuale intersezione che si ha tra due [[Eventi]] sommati tra loro:
>[!definizione] Definizione
>$\forall E,F\subset \Omega$ allora $\mathbb{P}(E\cup F)=\mathbb{P}(E)+\mathbb{P}(F)-\mathbb{P}(E\cap F)$,

Questo perché:

![[Inclusione-Esclusione.excalidraw]]

Da questa figura notiamo subito che se calcolassimo la probabilità di $E+F$ ci ritroveremo con 2 volte la probabilità di $C$, formalizzandolo:

(Dando per scontato che $A\cap B=\emptyset,B\cap C=\emptyset,A\cap C=\emptyset$):

$\mathbb{P}(E\cup F)=\mathbb{P}(A\cup B\cup C)=\mathbb{P}(A)+\mathbb{P}(B)+\mathbb{P}(C)$
- $\mathbb{P}(E)=\mathbb{P}(A\cup B)=\mathbb{P}(A)+\mathbb{P}(B)$
- $\mathbb{P}(F)=\mathbb{P}(B\cup C)=\mathbb{P}(B)+\mathbb{P}(C)$
Già qua notiamo che stiamo contando $\mathbb{P}(B)$ 2 volte