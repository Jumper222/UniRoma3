#Probabilità_e_statistica 
>[!Definizione]  Definizione
>La disuguaglianza di Markov è una stima che utilizziamo quando un problema ci da il [[Valore Atteso]] e ci chiede la probabilità che un valore maggiore o uguale ad un dato X si verifichi, ed ha la formula:
>$$\mathbb{P}(X\geq a)\leq \dfrac{\mathbb{E}[X]}{a}$$

Facciamo un esempio:

Abbiamo una fabbrica che produce 50 componenti ogni settimana, qual’è la possibilità ne produca 75?
Il problema ci da solo il valore assoluto, ossia $\mathbb{E}[X]=50$
Qui allora usiamo la disuguaglianza di Markov: 
$\mathbb{P}(X\geq 75)\leq \dfrac{\mathbb{E}}{75}=\dfrac{50}{75}=\dfrac{2}{3}=66.6\%$
