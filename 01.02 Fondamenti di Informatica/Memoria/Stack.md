Lo <font color="#ffff00">stack</font> è una “pila”, che tiene conto di tutti i “record di attivazione” delle <font color="#f79646">funzioni</font>, ossia dei blocchi di memoria che tengono conto dei dati necessari all’ esecuzione e attivazione di una funzione, tra cui le variabili locali.

Questo <font color="#ffff00">stack</font> tiene dentro di se ogni funzione “attiva”, ossia una funzione invocata ma non ancora terminata.

Quando una nuova funzione $f$ viene invocata, essa si aggiungerà in cima allo <font color="#ffff00">stack</font>, allocando la necessaria memoria. Quando questa funzione terminerà la sua memoria verrà deallocata.

La dimensione dello <font color="#ffff00">stack</font> è decisa alla compilazione del programma

<font color="#ff0000">!!!</font> In ogni momento, la funzione in cima dello <font color="#ffff00">stack</font> è quella in esecuzione.

Se una funzione, o una variabile dentro essa dovesse chiedere troppe risorse (come un array con $10^6$ elementi), potrebbe essere superata la capacità dello <font color="#ffff00">stack</font>, e si andrebbe in uno <font color="#e36c09">Stack Overflow</font>