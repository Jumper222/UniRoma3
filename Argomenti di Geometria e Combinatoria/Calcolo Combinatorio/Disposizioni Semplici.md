Una disposizione semplice, o senza ripetizione è il più semplice tipo di Disposizione, infatti si utilizza per calcolare ad esempio il numero di parole che si possono ottenere usando k lettere di una parola con n lettere.

### <font color="#4f81bd">Esempio</font>:

Prendiamo in considerazione la parola Giovane, con $n=7$ lettere, e diamogli una classe di $k=4$

Si inizi considerando che le lettere sono 7 distinte tra loro.
Allora dovremmo creare una serie di parola con 4 lettere ognuna, senza lettere che si ripetono al loro interno.
Possiamo quindi dire che una parola cambia da un’ altra se varia almeno una lettera tra le 2.

Allora possiamo descrivere la struttura del problema:
$$D_{7,4}=\frac{7!}{(7-4)!}=\frac{7!}{3!}=\frac{5040}{6}=840$$
E se volessimo generalizzare la formula:
$$D_{n,k}=\frac{n!}{(n-k)!}$$
