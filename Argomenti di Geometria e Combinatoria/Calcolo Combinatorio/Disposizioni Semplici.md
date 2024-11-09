Una disposizione semplice, o senza ripetizione è il più semplice tipo di Disposizione, infatti si utilizza per calcolare ad esempio il numero di parole che si possono ottenere usando k lettere di una parola con n lettere.

### <font color="#4f81bd">Esempio 1</font>:

Prendiamo in considerazione la parola Giovane, con $n=7$ lettere, e diamogli una classe di $k=4$

Si inizi considerando che le lettere sono 7 distinte tra loro.
Allora dovremmo creare una serie di parola con 4 lettere ognuna, senza lettere che si ripetono al loro interno.
Possiamo quindi dire che una parola cambia da un’ altra se varia almeno una lettera tra le 2.

Allora possiamo descrivere la struttura del problema:
$$D_{7,4}=\frac{7!}{(7-4)!}=\frac{7!}{3!}=\frac{5040}{6}=840$$
E se volessimo generalizzare la formula:
$$D_{n,k}=\frac{n!}{(n-k)!}$$


### <font color="#4f81bd">Esempio 2</font>:

Vediamo ora un esempio di una disposizione semplice più complicata:

In un sacchetto abbiamo 13 palline numerate, in quanti modi si possono estrarre 8 palline una dopo l’ altra se l’ estrazione avviene senza reimmissione?

Qui bisogna notare immediatamente la natura del problema: infatti come dati avremo $n=13$ e $k=8$

E cosi potremo calcolare il numero di disposizioni semplici amesse dal problema.
Ovvero:

$D_{13,8}=\frac{13!}{5!}=51.891.840$


<font color="#ff0000">NB</font>: Le disposizioni semplici possono essere viste come un caso particolare di permutazioni semplici, nel caso dove $n=k$
