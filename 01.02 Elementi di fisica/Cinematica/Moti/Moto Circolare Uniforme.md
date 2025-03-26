 #Elementi_di_Fisica 
>[!Definizione]  Definizione
>Il moto circolare uniforme (MCU) è un moto che agisce con una traiettoria che ha la forma di una circonferenza, è quindi un moto bidimensionale, che però possiamo rendere monodimensionale se prendiamo la circonferenza come traiettoria che percorriamo.
>Il MCU è un moto molto particolare, infatti abbiamo il concetto di:
>- Accelerazione centripeta (è una accelerazione che porta il corpo dentro la circonferenza
>- Velocità tangenziale (è una velocità che è tangente alla circonferenza)

Tabella per lookup veloce delle formule:

| Nome                      | Formula                                                         |
| ------------------------- | --------------------------------------------------------------- |
| Velocità angolare media   | $\omega=\dfrac{\Delta\theta}{\Delta t}$                         |
| Velocità tangenziale      | $v=r\omega$                                                     |
| Accelerazione centripeta  | $a_{c}=\dfrac{v^2}{r}=r\omega^2$                                |
| Accelerazione istantanea  | $\alpha=\lim_{ \Delta t \to 0 } \dfrac{\Delta\omega}{\Delta t}$ |
| Accelerazione tangenziale | $a_{t}=r\alpha\hat{\tau}$                                       |
Nel moto circolare uniforme abbiamo sempre che 


E se invece volessimo ottenere la velocità o accelerazione dalla posizione:

<font color="#ffff00">Posizione</font>:
$$r(t)=\begin{cases}x(t)=R\cos(\theta(t)) \\
y(t)=R\sin(\theta(t))
\end{cases}$$
<font color="#ffff00">Velocità</font>: (Qui $\theta'(t)$ è la velocità angolare)
$$v(t)=\begin{cases}
x(t)=-R\sin(\theta(t))*\theta'(t) \\
y(t)=R\cos(\theta(t))*\theta'(t)
\end{cases}$$
<font color="#ffff00">Accelerazione</font>: (la prima parte è l’ accelerazione centripeta, la seconda quella tangenziale)
$$a(t)=R\begin{cases}
x(t)=-\cos(\theta(t))*\theta'(t)^2-\sin (\theta(t))*\theta''(t) \\
y(t)=-\sin(\theta(t))*\theta'(t)^2+\cos(\theta)(t)*\theta''(t)
\end{cases}$$Iniziamo:
Il vettore posizione nel moto armonico appare graficamente:


![[MCU.excalidraw]]

Ed è descritto algebricamente dalle seguenti formule:

- <font color="#f79646">Coordinate cartesiane</font>:
$$\vec{r}(t)=R\cos[\theta(t)]\hat{x}+R\sin[\theta(t)]\hat{y}$$
- <font color="#f79646">Coordinate polari</font>: (Questo modo di scrivere è anche inteso come direzione radiale)
$$\vec{r}(t)=R\hat{v}(t)$$ 
Come ben sappiamo possiamo ottenere la velocità derivando la posizione:
per quanto riguarda le <font color="#f79646">coordinate cartesiane</font>:
$$\vec{v}(t)=\dfrac{d\vec{r}(t)}{dt}=-R\sin(\theta(t))\ \dfrac{d\theta(t)}{dt}\hat{x}+R\cos(\theta(t))\ \dfrac{d(\theta(t))}{dt}$$
E invece per quanto riguarda le <font color="#f79646">coordinate polari</font>:
$$\vec{v}(t)=\dfrac{d\vec{r}(t)}{dt}=R*w(t)*\underbrace{[-\sin \theta(t)\hat{x}+\cos \theta(t)\hat{y}]}_{\hat{\tau}(t)}$$
Qui la seconda parte la chiamiamo $\hat{\tau}(t)$

Abbiamo anche la seguente formula:
$$\theta(t)\to \omega (t)=\dfrac{d\theta(t)}{dt}$$
Questa è anche detta <font color="#ffff00">velocità angolare</font>, però non coincide con la pulsazione nonostante abbia lo stesso simbolo

Quando andiamo a calcolare la $\vec{v}(t)$ otteniamo che questo vettore è perpendicolare a quello della posizione, e di conseguenza anche l’ accelerazione è perpendicolare alla velocità, quindi sarà opposta al vettore posizione.

E allora $\vec{a}(t)=R(\dfrac{d\omega(t)}{dt}*\tau(t)+\dfrac{\omega(t)*d\tau(t)}{dt})$

quindi abbiamo infine le formule:
$$\dfrac{d\vec{\tau}(t)}{dt}=-\omega(t) \hat{v}(t)$$
allora abbiamo la formula per l’ accelerazione:
$$\vec{a}(t)=R\alpha(t)*\hat{\tau}(t)-R\omega(t)^2*\hat{v}(t)$$
la prima parte della formula è la velocità tangenziale e la parte destra è l’ accelerazione centripeta. 