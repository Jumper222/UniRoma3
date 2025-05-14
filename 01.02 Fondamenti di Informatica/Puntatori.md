---
tags:
  - Fondamenti_di_Informatica
---
Un puntatore è un particolare tipo di <font color="#9bbb59">variabile</font>, dentro al quale viene salvato l’ indirizzo di memoria di un’ altra <font color="#9bbb59">variabile</font>.

L’ indirizzo di memoria che ci andiamo a salvare indica il primo byte di quelli che sono associati alla <font color="#9bbb59">variabile</font> puntata

Ed ha la sintassi:
<font color="#f79646">tipoPuntato</font> <font color="#9bbb59"><font color="#4bacc6">*nome_puntatore</font></font>

Quindi ad esempio per un puntatore ad un intero:

```c
int *PuntatoreIntero;
int Intero=20;
PuntatoreIntero = &Intero;
```

In questo caso abbiamo <font color="#4bacc6">PuntatoreIntero</font> che viene dichiarato come puntatore di interi (riga 1)
Poi <font color="#4bacc6">Intero</font> viene dichiarato come intero con valore = 20 (riga 2)
Infine assegniamo a <font color="#4bacc6">PuntatoreIntero</font> l’ indirizzo di <font color="#4bacc6">Intero</font>, questo avviene grazie all’ operatore &, che si occupa di dare il valore dell’ indirizzo di memoria della variabile invece del suo valore.


Ora però dentro a <font color="#4bacc6">PuntatoreIntero</font> abbiamo soltanto un indirizzo, e questo non ci è molto utile al momento, infatti se volessimo ottenere il valore di <font color="#4bacc6">Intero</font> da <font color="#4bacc6">PuntatoreIntero</font> dovremmo usare l’ <font color="#f79646">Operatore di Indirezione (*)</font>

Allora adesso possiamo fare:

```C
printf("Abbiamo il valore: %d", *PuntatoreIntero);
```

Questo speciale operatore però è utilizzabile solo con le variabili di tipo puntatore.
Adesso inoltre possiamo dire che le due variabili <font color="#4bacc6">Intero</font> e <font color="#4bacc6">PuntatoreIntero</font> sono equivalenti.

Questi sono tutti esempi di puntatori con un tipo, però possiamo anche usare [[Puntatori Generici]]