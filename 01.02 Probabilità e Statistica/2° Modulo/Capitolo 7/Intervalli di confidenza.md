---
tags:
  - Probabilità_e_statistica
---

Utilizzare gli Intervalli di confidenza si rivela utile quando ci serve una <font color="#c0504d">stima per quanto sia giusta la nostra stima</font>

>[!Definizione]  Definizione
>Poniamo di avere un [[Campione Aleatorio]] $(x_{1},\dots,x_n)$ [[IID]] con [[Gaussiana Standard|Distribuzione Normale]] $\mathcal{N}(0,1)$, 
>Allora abbiamo la confidenza $1-\alpha$, con $\alpha\in(0,1)$, con cui possiamo trovare 3 tipi di intervalli per la media:
>- Intervallo di confidenza $(1-\alpha)*100\%$ bilaterale per la media:
>$$\mathbb{P}\left(\mu\in\left[\bar{X}-Z_{\dfrac{\alpha}{2}}* \dfrac{\sigma}{\sqrt{ n }},\bar{X}+Z_{\dfrac{\alpha}{2}}* \dfrac{\sigma}{\sqrt{ n }}\right]\right)$$
>- Intervallo di confidenza $(1-\alpha)*100\%$ unilaterale destro per la media:
>$$\mathbb{P}\left(\mu\in \left(\bar{X}-Z_{\alpha}* \dfrac{\sigma}{\sqrt{ n }},\infty \right) \right)$$
>- Intervallo di confidenza $(1-\alpha)*100\%$ unilaterale sinistro per la media:
>$$\mathbb{P}\left(\mu\in \left(\infty,\bar{X}+Z_{\alpha}* \dfrac{\sigma}{\sqrt{ n }} \right) \right)$$

Se non avessimo $\sigma$ dato, allora useremmo invece:

![[sigma ignota.png]]

Allo stesso modo possiamo trovare altri valori oltre la media:

![[Intervalli di confidenza (varianza).png]]

![[Intervalli di confidenza (Formule varianza).png]]

Per quanto riguarda invece la differenza delle medie di due popolazioni normali:

![[Intervalli di confidenza (Differenza medie).png]]