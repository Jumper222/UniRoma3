#Probabilità_e_statistica 
>[!Definizione]  Definizione
>Una [[Variabili Aleatorie discrete e continue|v.a. Continua]] di parametri $\mu,\sigma^2$ (con $\mu\in\mathbb{R},\sigma^2>0$) avrà una [[Fun. di densità di Probabilità (PDF)|PDF]] nella forma:
>$$f_{X}(x)=\dfrac{1}{\sqrt{ 2\pi\sigma^2 }}e^{\dfrac{-((x-\mu)^2)}{2\sigma^2}}$$
>E si scrive $$X\sim N(\mu,\sigma^2)$$
>La PDF sarà nella forma:
>![[Gaussiana PDF.png]]
>Il [[Valore Atteso]] della gaussiana sarà:
>$$\mathbb{E}[X]=\mu$$
>E per quanto riguarda la [[Varianza]], essa sarà
>$$\sigma^2$$
>Questo è fantastico perché allora possiamo dire che media e [[varianza]] sono ottenibili direttamente dalla v.a: $X\sim \mathcal{N}(\mu,\sigma^2)$

Esattamente come le [[Variabili Aleatorie di Poisson|v.a. di Poisson]] le Gaussiane sono riproducibili, ossia se prendiamo due v.a. [[IID]]
e poniamo $Y=aX_{1}+bX_{2}$
Y rimarrà Gaussiana, e avrà valori notevoli:

[[Valore Atteso]]:
$$\mathbb{E}(Y)=a\mu_{1}+b\mu_{2}$$
e la [[Varianza]]:
$$Var(Y)=a^2\sigma^2_{1}+b^2\sigma^2_{2}$$


La Gaussiana è unica perché ha varie particolarità:
- Sappiamo inoltre che al variare di $\mu$, con $\sigma^2$ fissato si ottiene una traslazione della curva
- Il punto di massimo è in $x=\mu$ in cui $f_{X}=\dfrac{1}{\sqrt{ 2\pi \sigma^2 }}\approx \dfrac{0.399}{\sigma}$
- $f_{X}$ è simmetrica rispetto a $\mu: f_{X}(\mu+x)=f_{X}(\mu-x)$

Un’ altra proprietà fondamentale della gaussiane è anche la seguente:

### <font color="#4bacc6">Gaussiana composta</font>

Se $X\sim N(\mu,\sigma^2),Y=aX+b$
Allora Y sarà distribuita come:
$$Y\sim N(a\mu+b,a^2\sigma^2)$$

---

Molte volte quando useremo una v.a. Gaussiana avremo una [[Gaussiana Standard]]