Certamente. Una variabile aleatoria uniforme è un tipo di variabile aleatoria in cui tutti i valori all'interno di un intervallo specificato hanno la stessa probabilità di verificarsi

. Le fonti si concentrano principalmente sulla variabile aleatoria uniforme continua.

Variabile Aleatoria Uniforme Continua

Una variabile aleatoria continua $X$ si dice uniforme sull'intervallo $[a, B]$, dove $a < B$, se la sua funzione di densità di probabilità (PDF) è data da

:

$f_X(x) = \begin{cases} \frac{1}{B-a} & \text{per } a \le x \le B \ 0 & \text{altrimenti} \end{cases}$

dove $a$ e $B$ sono i parametri della distribuzione e rappresentano rispettivamente l'estremo inferiore e superiore dell'intervallo

. La PDF è costante sull'intervallo $[a, B]$ e zero al di fuori di esso. Questo significa che la probabilità che la variabile aleatoria cada in un qualsiasi sottointervallo di $[a, B]$ dipende solo dalla lunghezza di quel sottointervallo e non dalla sua posizione

.

La funzione di ripartizione (CDF) $F_X(x) = P(X \le x)$ per una variabile aleatoria uniforme su $[a, B]$ è

:

$F_X(x) = \begin{cases} 0 & \text{per } x < a \ \frac{x-a}{B-a} & \text{per } a \le x \le B \ 1 & \text{per } x > B \end{cases}$

Il valore atteso (media) di una variabile aleatoria uniforme su $[a, B]$ è

:

$E[X] = \int_{-\infty}^{\infty} x f_X(x) dx = \int_{a}^{B} x \frac{1}{B-a} dx = \frac{a+B}{2}$

Questo significa che la media della distribuzione uniforme si trova esattamente a metà dell'intervallo $[a, B]$

.

La varianza di una variabile aleatoria uniforme su $[a, B]$ è

:

$Var(X) = E[X^2] - (E[X])^2 = \frac{(B-a)^2}{12}$

dove $E[X^2] = \int_{a}^{B} x^2 \frac{1}{B-a} dx = \frac{a^2 + aB + B^2}{3}$

.

Esempio

Consideriamo l'esempio in cui un autobus passa ogni 15 minuti a partire dalle 7:00 (quindi alle 7:00, 7:15, 7:30...)

. Se si arriva alla fermata in un istante di tempo uniformemente a caso tra le 7:00 e le 7:30, possiamo modellare il tempo di arrivo in minuti dopo le 7:00 con una variabile aleatoria $X \sim Unif$

.

La probabilità di aspettare meno di 5 minuti si verifica se si arriva tra le 7:10 e le 7:15 oppure tra le 7:25 e le 7:30

. La probabilità è quindi la somma delle probabilità di cadere in questi due intervalli di lunghezza 5 minuti ciascuno, all'interno di un intervallo totale di 30 minuti

:

$P(\text{aspettare } < 5 \text{ minuti}) = P(10 < X < 15) + P(25 < X < 30)$

$P(10 < X < 15) = \int_{10}^{15} \frac{1}{30} dx = \frac{15-10}{30} = \frac{5}{30}$

$P(25 < X < 30) = \int_{25}^{30} \frac{1}{30} dx = \frac{30-25}{30} = \frac{5}{30}$

$P(\text{aspettare } < 5 \text{ minuti}) = \frac{5}{30} + \frac{5}{30} = \frac{10}{30} = \frac{1}{3}$

Le variabili aleatorie uniformi su $

$ sono particolarmente importanti perché possono essere utilizzate per simulare il comportamento di qualsiasi altra variabile aleatoria tramite il metodo dell'inversione.