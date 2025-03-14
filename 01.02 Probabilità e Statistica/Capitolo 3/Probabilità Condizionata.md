#Probabilità_e_statistica 
>[!Definizione]  Definizione
>$\forall E,F\subset \Omega\ | \ F\neq \emptyset$ chiamiamo “Probabilità di $E$ dato $F$”:
>$$\mathbb{P}(E|F)=\frac{\mathbb{P}(E\cap F)}{\mathbb{P}(F)}$$

La Probabilità Condizionata è un particolare tipo di [[Funzione di probabilità|probabilità]], dove diamo per scontato che un determinato evento si verifichi.

Questo implica che lo [[Spazio campionario]] si riduca, divenendo grande quanto $\mathbb{P}(F)$:
![[Probabilità Condizionata.excalidraw]]
*In marrone sono tutti gli eventi non considerati*

---

<font color="#e36c09">NOTA</font>: Poiché $\forall E,F\subset \Omega$ con $F\neq \emptyset$, allora abbiamo che:
$$\mathbb{P}(E|F)=\frac{\mathbb{P}(E\cap F)}{\mathbb{P}(F)}$$
Posso quindi calcolare che la probabilità di $E\cap F$:
$$\mathbb{P}(E\cap F)=\mathbb{P}(F)*\mathbb{P}(E|F)$$
---
<font color="#e36c09">NOTA</font>: Poiché $\forall E,F\subset \Omega$, con $F\neq \emptyset$, Abbiamo che:
$$E={\color{Cyan} \underline{(E\cap F)}}\cup {\color{Orange} \underline{(E\cap F^c)}}$$
![[Probabilità Condizionata disgiunzione.excalidraw]]

(Questa formula ha senso visto che $E\cap F$ e $E\cap F^c$ sono disgiunti)

Facciamo qualche esempio:

[[Esempi sulla probabilità condizionata]]