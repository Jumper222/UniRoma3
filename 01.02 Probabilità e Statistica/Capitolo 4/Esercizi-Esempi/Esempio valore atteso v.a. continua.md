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

![[Esempio valore atteso v.a. continua.png]]

Allora calcoliamo il valore atteso, ricordandoci che:
- $\frac{3}{2}$= tempo totale d’ attesa, in ore
- $\frac{2}{3}$= possibilità che otteniamo 