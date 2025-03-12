#Probabilità_e_statistica 
>[!Definizione]  Definizione
>Se $X$ è una [[Variabili aleatorie discrete e continue|v.a. discreta]] chiamo [[Funzioni|Funzione]] di massa di probabilità </font> (anche detta PMF in inglese), alcune volte scritta $P_{x}$ La funzione che associa a ciascun valore (che $X$ può assumere) la probabilità che $X$ assuma quel valore, ed è definita tale che:
>$$p:\mathrm{Im}(X)\to[0,1]$$

Facciamo un esempio:
$X$ è la somma dei risultati del lancio di due dadi:
- $p(2)=\frac{1}{36}$ (La possibilità che escano 2 dadi che sommati diano 2)
- $p(3)=\frac{2}{36}$
- $p(4)=\frac{3}{36}$
- $p(5)=\frac{4}{36}$
- $p(6)=\frac{5}{36}$
- $p(7)=\frac{6}{36}$
- $p(8)=\frac{5}{36}$
- $p(9)=\frac{4}{36}$
- $p(10)=\frac{3}{36}$
- $p(11)=\frac{2}{36}$
- $p(12)=\frac{1}{36}$

Quindi sarà in questa forma:

![[Funzione di massa di probabilità (brutta).png]]

Oppure meglio conosciuta in questa forma:

![[Esempio 1 funzione di massa di probabilità.png]]

Queste rappresentazioni ci dicono quante possibilità ci sono che la somma dei due dadi dia il numero indicato con le $x$.

Facciamo un secondo esempio:

### Esempio 2:

Supponiamo che quando calcio un rigore ho prob. di $\frac{2}{3}$ di fare gol, e che gli esiti relativi a rigori distinti siano indipendenti.

Allora avremo:
$X=\text{ \# rigori che calcio finché non segno}$
$\mathrm{Im}(X)=\mathbb{N}=\{1,2,3\dots\}$

Quindi: 
$p(1)=\mathbb{P}(X=1)=\frac{2}{3}$
$p(2)=\mathbb{P}(X=2)=\left( 1-\frac{2}{3} \right) \frac{2}{3}$
$p(n)=\mathbb{P}(X=n)=\left( 1-\frac{2}{3} \right)^{n-1} \frac{2}{3}$

Cosi otterremo una serie andando ad infinito che ci darà questi grafici:

![[Esempio funzione di massa di probabilità.png]]

Notiamo subito come questi grafici rappresentino come la probabilità si avvicini sempre di più ad essere 1 più tiri facciamo.

Da qui deduciamo che se $X$ è una v.a. discreta possiamo ricavarne una seria tale che:
$$\sum_{y\in \mathrm{Im}(X)}Px(y)$$
