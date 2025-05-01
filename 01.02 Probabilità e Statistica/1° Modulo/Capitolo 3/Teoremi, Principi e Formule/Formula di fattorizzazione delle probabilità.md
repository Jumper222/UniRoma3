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
Se è caduto nella regione $i\in\{1,2,3\}$ ho probabilità $\alpha_{i}$ di trovarlo cercando nella regione $i$.
Allora si ha l’ evento $E$ “cerco l’ aereo nella regione 1 e non lo trovo”
$\mathbb{P}(E|R_{1})=\alpha_{1}$, allora $\mathbb{P}(E|R_{2})=\mathbb{P}(E|R_{3})=1$ (o sta in uno o nell’ altro)

$$\mathbb{P}(R_{1}|E)=\frac{\mathbb{P}(E|R_{1})\mathbb{P}(R_{1})}{\mathbb{P}(E)}=\frac{\alpha_{1}* \frac{1}{3}}{\sum^3_{i=1}\mathbb{P}(R_{i})\mathbb{P}(E|R_{i})}=\frac{\alpha_{1}* \frac{1}{3}}{\alpha_{1}* \frac{1}{3}+ 1* \frac{1}{3}+1* \frac{1}{3}}$$
Abbiamo un ragionamento simile per $R_{2,3}$:
$$\mathbb{P}(R_{2}|E)=\frac{\mathbb{P}(E|R_{2})\mathbb{P}(R_{2})}{\mathbb{P}(E)}=\frac{1* \frac{1}{3}}{\sum^3_{i=1}\mathbb{P}(R_{i})\mathbb{P}(E|R_{i})}=\frac{1* \frac{1}{3}}{\alpha_{1}* \frac{1}{3}+ 1* \frac{1}{3}+1* \frac{1}{3}}$$
