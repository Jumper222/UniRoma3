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
Già qua notiamo che stiamo contando $\mathbb{P}(B)$ 2 volte, continuiamo:
- $\mathbb{P}(E\cup F)=\mathbb{P}(E)+\mathbb{P}(F)-\mathbb{P}(B)$, Allora:
- $\mathbb{P}(E)+\mathbb{P}(F)-\mathbb{P}(E\cap F)$
<font color="#ffff00">Dimostrazione  finita!</font>

Facciamo un semplice esempio:

In una classe:
- il $28\%$ delle persone fumano sigarette
- il $7\%$ IQOS
- il $5\%$ sigarette ed IQOS

Allora definiamo:
- $E$: è fumatore di sigarette
- $F$: è fumatore di IQOS
- $E\cap F$ è fumatore di sigarette e di IQOS

<font color="#f79646">Domanda</font>: Qual’è la possibilità che la persona scelta non fumi?
Per risolvere l’ esercizio dovremo calcolare $(E\cup F)^c$:
$\mathbb{P}(E\cup F)=\mathbb{P}(E)+\mathbb{P}(F)-\mathbb{P}(E\cap F)$ → (Questo è il [[Principio di inclusione-esclusione]])
Quindi: $0,28+0,07-0,05=0,3$
Allora $\mathbb{P}((E\cup F)^c)=1-\mathbb{P}(E\cup F)=1-0,3=0,7$