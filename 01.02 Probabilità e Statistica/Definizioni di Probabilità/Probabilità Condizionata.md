#Probabilità_e_statistica 

>[!Definizione]  Definizione
>$\forall E,F\subset \Omega\ | \ F\neq \emptyset$ chiamiamo “Probabilità di $E$ dato $F$”:
>$$\mathbb{P}(E|F)=\frac{\mathbb{P}(E\cap F)}{\mathbb{P}(F)}$$

La Probabilità Condizionata è un particolare tipo di [[Funzione di probabilità|probabilità]], dove diamo per scontato che un determinato evento si verifichi.

Questo implica che lo [[Spazio campionario]] si riduca, divenendo grande quanto $\mathbb{P}(F)$:
![[Probabilità Condizionata.excalidraw]]
*In marrone sono tutti gli eventi non considerati*

---

Facciamo qualche esempio:
### <font color="#4bacc6">Esempio 1</font>:

Lancio 2 dadi, uno rosso ed uno blu, allora:
$|\Omega|=6*6=36$ 
Supponiamo che gli eventi siano equiprobabili,
$E$: “La somma dei dadi da 8”=$\{(2,6),(3,5),(4,4),(5,3),(6,2)\}$
Abbiamo quindi che $\mathbb{P}(E)=\frac{5}{36}$
