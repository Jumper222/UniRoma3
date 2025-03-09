#Probabilità_e_statistica 
>[!Definizione]  Definizione
>Possiamo descrivere la probabilità di un qualsiasi evento se sono note le probabilità condizionate rispetto ad un gruppo di eventi, che sono esclusivi tra loro, che rappresentano una partizione di tutto $\Omega$:
>$\forall E \subset \Omega$:
>$$E=\bigcup^n_{i=1}(E\cap F) \ (\text{rappresenta l' unione disgiunta})$$
>Allora:
>$$\mathbb{P}(E)=\sum^n_{i=1}\mathbb{P}(E\cap F_{i})=\sum^n_{i=1}\mathbb{P}(F_{i})\mathbb{P}(E|F_{i})$$

Appare quindi in questa forma:
![[Fattorizzazione di un Evento.excalidraw]]

Facciamo un esempio:

Un aereo è scomparso in una di 3 regioni (con uguale probabilità)
$\mathbb{P}(R_{1})=\mathbb{P}(R_{2})=\mathbb{P}(R_{3})=\frac{1}{3}$
Se è caduto nella regione $i\in\{1,2,3\}$ ho probabilità $\alpha_{i}$ di trovarlo