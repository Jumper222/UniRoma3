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
Supponiamo che gli eventi siano equiprobabili, Consideriamo l’ evento $E$:

$E$: “La somma dei dadi da 8”=$\{(2,6),(3,5),(4,4),(5,3),(6,2)\}$
Abbiamo quindi che $\mathbb{P}(E)=\frac{5}{36}$

Ora  consideriamo un evento $F$: 

$F$: “Il dado rosso da 3” = $\{(3,1),(3,2),(3,3),(3,4),(3,5),(3,6)$

Quanto vale $\mathbb{P}(E)$ se so che $F$ si verifica?

Varrà $\frac{1}{6}$, che deriva dalla formula iniziale.

---

### <font color="#4bacc6">Esempio 2</font>:

In una scatola ho $40$ componenti elettroniche
- $5$ guaste (non funzionano)
- $10$ difettose (funzionano per $1h$ e poi si rompono)
- $25$ accettabili (funzionano)

Allora scelgo una componente a caso:
- $G$: è guasta
- $D$: è difettosa
- $A$: è accettabile

$\mathbb{P}(G)=\frac{5}{40}$
$\mathbb{P}(D)=\frac{10}{40}$
$\mathbb{P}(A)=\frac{25}{40}$

Ora supponiamo che inizialmente la componente funzioni → $D\cup A=G^c$
Quale sarà la probabilità di $A$?

