---
tags:
  - Fondamenti_di_Informatica
share_link: https://share.note.sx/4m9knno2#U/IKk4DcIVJaFYKfCugnDXOY2uAt40bh89hfZpbd7PE
share_updated: 2025-05-14T18:29:29+02:00
---
Un puntatore è un particolare tipo di <font color="#9bbb59">variabile</font>, dentro al quale viene salvato l’ indirizzo di memoria di un’ altra <font color="#9bbb59">variabile</font>.

L’ indirizzo di memoria che ci andiamo a salvare indica il primo byte di quelli che sono associati alla <font color="#9bbb59">variabile</font> puntata

Ed ha la sintassi:
<font color="#f79646">tipoPuntato</font> <font color="#9bbb59"><font color="#4bacc6">*nome_puntatore</font></font>

Quindi ad esempio per un puntatore ad un intero:

```c
int *Puntatore;       // Dichiariamo un Puntatore di Interi
int Intero=20;        // Inizializziamo un intero con valore = 20
Puntatore = &Intero;  // Assegniamo a Puntatore l' indirizzo della variabile Intero
```

Ora però dentro a <font color="#4bacc6">Puntatore</font> abbiamo soltanto un indirizzo, e questo non ci è molto utile al momento, infatti se volessimo ottenere il valore di <font color="#4bacc6">Intero</font> da <font color="#4bacc6">Puntatore</font> dovremmo usare l’<font color="#f79646">Operatore di Indirezione (*)</font>

Allora adesso possiamo fare:

```C
printf("Abbiamo il valore: %d", *Puntatore);
```
*Questo operatore è utilizzabile solo con le variabili di tipo puntatore.*

Adesso inoltre possiamo dire che le due variabili <font color="#4bacc6">Intero</font> e <font color="#4bacc6">PuntatoreIntero</font> sono equivalenti.

Questi sono tutti esempi di puntatori con un tipo, però possiamo anche usare [[Puntatori Generici]]

Un comune uso dei puntatori è riguardante gli [[Puntatori ed Array]]

##### Puntatori <font color="#9bbb59">selvaggi</font> e <font color="#9bbb59">pendenti</font>

Questi due tipi di puntatori sono potenzialmente dannosi, in quanto imprevedibili (Puntano ad aree di RAM non allocate, quindi potenzialmente usate da altri software.) 

I puntatori che sono stati dichiarati ma non inizializzati si dicono <font color="#ffff00">Wild Pointers</font> (<font color="#9bbb59">Selvaggi</font>)
In particolare ogni volta che dichiariamo un puntatore è <font color="#d99694">buona norma</font> inizializzarli con ‘<font color="#ffc000">NULL</font>’

I puntatori che puntano ad una area di memoria senza valori utili al programma si chiama <font color="#ffff00">Dangling Pointer</font>(<font color="#9bbb59">Pendenti</font>),
Si hanno quando creiamo dei <font color="#c4bd97">puntatori</font> a variabili dentro una <font color="#f79646">funzione</font>, che poi una volta finita <font color="#4bacc6">dealloca</font> tutta la memoria delle variabili dichiarate al suo interno, tra cui quella a cui stiamo puntando

