---
tags:
  - Probabilità_e_statistica
---

Utilizzare gli Intervalli di confidenza si rivela utile quando ci serve una <font color="#c0504d">stima per quanto sia giusta la nostra stima</font>

>[!Definizione]  Definizione
>Poniamo di avere un [[Campione Aleatorio]] $(x_{1},\dots,x_n)$ [[IID]] con [[Gaussiana Standard|Distribuzione Normale]] $\mathcal{N}(0,1)$, 
>Allora abbiamo la confidenza $1-\alpha$, con $\alpha\in(0,1)$, con cui possiamo trovare 3 tipi di intervalli:
>- Intervallo di confidenza $(1-\alpha)*100\%$ bilaterale per la media:
>$$\mathbb{P}\left(\mu\in\left[\bar{X}-Z_{\dfrac{\alpha}{2}}* \dfrac{\sigma}{\sqrt{ n }},\bar{X}+Z_{\dfrac{\alpha}{2}}* \dfrac{\sigma}{\sqrt{ n }}\right]\right)$$
>- Intervallo di confidenza $(1-\alpha)*100\%$ unilaterale destro per la media:
>$$\mathbb{P}\left(\mu\in \left(\bar{X}-Z_{\alpha}* \dfrac{\sigma}{\sqrt{ n }},\infty \right) \right)$$
>- Intervallo di confidenza $(1-\alpha)*100\%$ unilaterale sinistro per la media:
>$$$$