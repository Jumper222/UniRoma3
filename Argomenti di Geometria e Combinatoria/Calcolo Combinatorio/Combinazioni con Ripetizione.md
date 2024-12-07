#Geometria_e_Combinatoria 
Una combinazione con ripetizione è un tipo di raggruppamento di classe k di un insieme con elementi n
Dove gli elementi si possono ripetere.

La formula per calcolarlo è:
$$C'_{n,k}=\frac{(n+k-1)!}{k!(n-1)!}$$
Anche qui è importante avere a mente il concetto di Coefficiente binomiale, infatti si usa anche la scrittura:
$$\binom{n+k-1}{k}$$

Entrambe le scritture indicano la stessa cosa.

### <font color="#4f81bd">Esempio</font>:

Un’ urna contiene 20 palline numerate. in quanti modi si possono estrarre 3 palline, supponendo che dopo ogni singola estrazione la pallina venga rimessa dentro l’ urna, e senza tener conto dell’ ordine con cui le palline sono state estratte?

<font color="#ffff00">Svolgimento</font>: abbiamo n=20 elementi distinti e dobbiamo stabilire quanti sono i raggruppamenti non ordinati formati da k=3 elementi estratti dagli n.

Poiche dopo ogni estrazione la pallina viene rimessa nell’ urna, una stessa pallina può essere estratta fino ad un massimo di 3 volte, dunque usiamo la formula delle combinazioni con ripetizione:
$$\binom{n+k-1}{k}$$
E vi sostituiamo n=20 e k=3:
$$C'_{20,3}=\binom{20+3-1}{3}=\binom{22}{3}=\frac{22!}{3!(22-3)!}=\frac{22!}{3!*19!}=1540$$
