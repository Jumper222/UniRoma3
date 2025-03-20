#Probabilità_e_statistica 
Supponiamo che stiamo aspettando una comunicazione che arriverà tra le 17:00 e le 18:30
Supponiamo inoltre che abbia la stessa possibilità di arrivare in qualsiasi istante di tempo.
Allora modellizziamo l’ esercizio con la PDF:
$$f_{X}(x)=\begin{cases}
\frac{1}{1.5} &  \text{se }x\in[0,1.5] \\
0  & \text{altrimenti}
\end{cases}$$
notiamo subito che $f_{x}$ è una PDF ben specificata, infatti il suo integrale tra 0 e 1.5 è proprio 1:
$$\int^{1.5}_{0}f_{X}(x)dx=\int^{1.5}_{0} \frac{1}{1.5}dx=1$$
Infatti il grafico è in questa forma:

![[01.02 Probabilità e Statistica/Immagini/Esempio valore atteso v.a. continua.png]]

Allora calcoliamo il valore atteso, ricordandoci che:
- $\frac{3}{2}$= tempo totale d’ attesa, in ore
- $\frac{2}{3}$= possibilità che otteniamo in ogni momento la comunicazione (1/tempo totale)

Il valore atteso sarà uguale a:
$$\mathbb{E}[X]=\int^ \frac{3}{2}_{0} \frac{2}{3}x\ dx=\frac{2}{3}\int^ \frac{3}{2}_{0}x\ dx=\dots=\frac{3}{4}$$
Possiamo quindi dire che in media aspetteremo <font color="#ffff00">45</font> min $\left( \frac{3}{4} h \right)$

Facciamo allora una variazione:

Supponiamo di avere un’ altra PDF:
$$f_{X}(x)=\begin{cases}
1- \frac{16}{9}\left( x-\frac{3}{4} \right)^2 & \text{se } x\in[0,1.5] \\
0 & \text{altrimenti}
\end{cases}$$
Innanzitutto controlliamo che sia ben definita, facendo l’ integrale tra $1.5 (\frac{3}{2})$ e $0$, se esso restituirà 1 potremo continuare.
$$\int^ \frac{3}{2}_{0}1-\frac{16}{9}\left( x-\frac{3}{4} \right)^2dx=\int^ \frac{3}{2}_{0} \left( 1-\frac{16}{9} x^2-1+\frac{8}{3}x \right)dx=\dots=1$$
Adesso la PDF assumerà un’ altra forma:

![[Esempio valore atteso v.a. continua 2.png]]

Allora calcoliamo ancora una volta il valore atteso:

$$\mathbb{E}[X]=\int^ \frac{3}{2}_{0} x\left( 1-\frac{16}{9} x^2-1+\frac{8}{3}x \right)dx=\dots=\frac{3}{4}$$
<font color="#f79646">NB</font>: Esattamente come nel caso in cui aveva una retta come PDF, anche con una parabola il valore atteso sarà al punto centrale.