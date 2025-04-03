#Probabilità_e_statistica 

>[!Definizione]  Definizione  
>Una Gaussiana Standard $Z$ è un particolare tipo di [[Variabili Aleatorie Gaussiane|v.a. Gaussiana]], è quindi [[Variabili Aleatorie discrete e continue|continua]], ed è definita:
>Se $X\sim N(\mu,\sigma^2)$
>Allora avremo
>$$Z=\dfrac{X-\mu}{\sigma}\sim N(0,1)$$
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

Però questo essendo la distribuzione