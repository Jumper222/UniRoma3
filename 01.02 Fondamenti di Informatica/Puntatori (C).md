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
Poi Intero viene dichiarato 
cosi che se facciamo un <font color="#ffc000">printf</font>() con <font color="#4bacc6">*PuntatoreIntero</font> ci esca 20.

Il motivo per cui usiamo 
