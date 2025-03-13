#Probabilità_e_statistica 
>[!Definizione]  Definizione
>I vettori di [[Variabili Aleatorie|v.a.]] (di cui le coppie o terne sono istanze con 2,3 dimensioni) sono appunto una generalizzazione del concetto di [[Variabili Aleatorie|v.a.]] che ci permette di descrivere situazioni in cui queste v.a. si intersecano.

Facciamo un esempio:
In una classe ci sono $100$ studenti:
- $30$ bravi in matematica ($24$ non bravi a programmare)
- $25$ bravi a programmare ($19$ non bravi in matematica)
- $6$ bravi sia in matematica che in programmazione

Allora scegliamo $7$ studenti a caso, siano:
- $X$= $\#$ studenti bravi in matematica tra quelli scelti
- $Y$= $\#$  studenti bravi in programmazione tra quelli scelti

Allora avremo che $\mathrm{Im}(X)=\{0\dots7\}=\mathrm{Im}(Y)$
Calcoliamo quindi $\mathbb{P}(X=2)$:
$$\frac{\binom{30}{2}\binom{70}{5}}{\binom{100}{7}}$$
*Ossia modi di scegliere 2 tra i 30 più bravi e 5 tra i 70 non bravi, diviso 7 scelti tra 100 totali*

E invece se volessimo calcolare $\mathbb{P}(Y=3)$ avremmo:
$$\frac{\binom{25}{3}\binom{75}{4}}{\binom{100}{7}}$$
A prima vista non sembrano eventi indipendenti.
$$\mathbb{P}(\{X=2\}\cap\{Y=3\})$$
Allora creiamo $Z$:  che sarà il numero di studenti bravi sia in programmazione che in matematica:
$\mathbb{P}(X=2)\mathbb{P}(Y=3|X=2)$
Allora abbiamo $\mathrm{Im}(Z)=\{0,\dots,6\}$

![[Coppie e vettori Esempio.png]]

![[Coppie e vettori v.a. img esempio 2.png]]

Molto spesso ci capiterà di avere esercizi dove siamo interessati ad una coppia di v.a. e di come sia il loro comportamento congiunto, qui entra in gioco la [[Funzione di ripartizione congiunta (CDF congiunta)|CDF congiunta]], e per le variabili continue avremo la [[Funzione di Densità Congiunta (PDF congiunta)|PDF congiunta]]

