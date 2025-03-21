#Probabilità_e_statistica 
>[!Definizione]  Definizione
>Il valore atteso, indicato con $\mathbb{E}(X)$ è il valore con cui descriviamo al meglio una [[Variabili Aleatorie|v.a.]],
>Esso ci fornisce il “baricentro” o media della [[Fun. di massa di Probabilità (PMF)]] della v.a. e assume vari nomi:
>- Valore atteso di X
>- Aspettazione di X
>- Media di X
>
>Ed è definito tale che:
>$$\mathbb{E}[X]=\sum_{x\in \mathrm{Im}(X)}x\ P_{X}(x)$$
>
>Per quanto riguarda le v.a. continue invece:
>$$\mathbb{E}[X]=\int^\infty_{-\infty}x\ f_{x}(x)dx$$
> Per le v.a. indicatrici invece abbiamo una [[Valore Atteso di una Variabile Aleatoria Indicatrice|specifica]]
>

> [!links]
>Potrebbe succedere che dobbiamo calcolare il [[Valore Atteso di una v.a. composta]]
>
>Esistono dei casi in cui ci potrebbe capitare di dover [[Calcolare il Valore Atteso di una funzione]]
>
>Invece potrebbe capitare di dover descrivere il [[Valore Atteso di 2+ v.a.]]
>
>Il Valore atteso è il primo momento della [[Funzione generatrice di momenti (MGF)]]


Se volessimo fare l’ esempio del lancio di un dado:
$\mathbb{E}[X]=1* \frac{1}{6}+ 2* \frac{1}{6} + \dots + 6* \frac{1}{6}=3.5$

![[Valore atteso.png]]
*In questa figura vediamo come il valore atteso è proprio 3.5*

Facciamo un secondo esempio:

Sia $X$ una v.a. descritta dalla sua PMF:
$$P_{X}(x)=\begin{cases}
0,2 \quad \text{se } x=1 \\
0,5 \quad \text{se } x=3 \\
0,3 \quad \text{se } x=7
\end{cases}$$
Allora il suo valore attesto sarà:
$$\mathbb{E}[X]=1*0.2+3*0.5+7*0.3=3.8$$
Ed il suo grafico in questa forma:

![[Esempio 2 valore atteso.png]]

Facciamo un esempio per il valore atteso di una v.a. continua: [[Esempio valore atteso v.a. continua]]

Il valore atteso poi ci permette di definire il concetto di [[Varianza]]