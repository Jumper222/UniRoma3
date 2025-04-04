#Probabilità_e_statistica 

>[!Definizione]  Definizione  
>Una Gaussiana Standard $Z$ è un particolare tipo di [[Variabili Aleatorie Gaussiane|v.a. Gaussiana]], è quindi [[Variabili Aleatorie discrete e continue|continua]], ed è definita:
>Se $X\sim N(\mu,\sigma^2)$
>Allora avremo
>$$Z=\dfrac{X-\mu}{\sigma}\sim \mathcal{N}(0,1)$$
>Ed avrà una [[Funzione di ripartizione congiunta (CDF congiunta)|CDF]] nella forma:
>$$F_{Z}(z)=\int^z_{-\infty} \dfrac{1}{\sqrt{ 2\pi }}e^{-\dfrac{x^2}{2}}=:\Phi(z)$$

*questo integrale non è risolvibile analiticamente, ma si può approssimare, infatti si ha una tabella:

![[Tabella Gaussiana.png]]

Per usare questa tabella ad esempio (viola):
$$\mathbb{P}(Z\leq-2.53)=\Phi(-2.53)\approx 0.0057$$
Questo numero lo otteniamo incrociando e cercando il valore che abbiamo con la virgola.
E allora abbiamo:

![[Gaussiana standard esempio viola.png]]

<font color="#ffff00">Attenzione però</font>!
La tabella ha soltanto i valori per $Z\leq 0$!

Vediamo l’ esempio blu:

$$\mathbb{P}(Z\leq 1.15)=1-\mathbb{P}(Z\leq -1.15)\approx 1-0.1251=0.8749$$


![[Gaussiana Standard esempio 2.png]]

Però essendo la gaussiana standard centrata sul [[valore atteso]] ed essendo uguale a destra e a sinistra, allora $\mathbb{P}(Z\leq 1.15)=\mathbb{P}(Z\leq -1.15)$

E se invece volessimo calcolare tra 2 valori (giallo)?

$$\mathbb{P}(Z\in[0.90,+1.32])=\ ?$$


![[Esempio 3 Gaussiana Standard.png]]

Molto semplicemente sottraiamo la probabilità del valore più piccolo a quello più grande:
$$\mathbb{P}(Z\leq 1.32)-\mathbb{P}(Z\leq -0.90)$$
$$1-0.0934-0.1841=0.7225$$


Più generalmente se $X\sim N(\mu,\sigma^2)$
allora avremo che:
$$\mathbb{P}(X\leq b)=\mathbb{P}(\dfrac{X-\mu}{\sigma}\leq \dfrac{b-\mu}{\sigma})=\Phi(\dfrac{b-\mu}{\sigma})$$
*Qui stiamo supponendo di non avere Z, e quindi generalizziamo su una [[Variabili Aleatorie Gaussiane|v.a. gaussiana]] generica*

E analogamente
$$\mathbb{P}(X\in(a,b))=\mathbb{P}(a<X<b)=\Phi(\dfrac{b-\mu}{\sigma})-\Phi(\dfrac{a-\mu}{\sigma})$$
---

### <font color="#4bacc6">Esempio</font>
Facciamo un esempio, poniamo che $X\sim N(3,16)$

Ora ci chiediamo:
$$\mathbb{P}(X<11)=\mathbb{P}(\dfrac{X-3}{4}< \dfrac{11-3}{4})$$
E allora, otterremo $\dfrac{8}{4}$ e quindi $\Phi(2)$
E per calcolare $\Phi(2)$ dobbiamo prima invertire:

$$1-\Phi(-2)\approx 1-0.0228=0.9772$$
Ora invece ci chiediamo $\mathbb{P}(X>-1)$:
$$\mathbb{P}(X>-1)=\mathbb{P}(\dfrac{-1-3}{4})=1-\Phi(-1)=1-0.1587=0.8413$$
Qui calcoliamo col -1 perché ci chiede il valore maggiore