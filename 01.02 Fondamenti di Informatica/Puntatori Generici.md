---
tags:
  - Fondamenti_di_Informatica
---
A differenza di un puntatore con un tipo, i <font color="#ffff00">puntatori</font> generici non possono accedere al valore della variabile indicata, alcune funzioni come <font color="#f79646">malloc()</font> ne fanno uso.

Per dichiarare un puntatore generico scriveremo:

```C
int a = 1;
char b = 'c'
void *Generico;
Generico = &a; // Gli assegniamo l' indirizzo di una variabile intera
Generico = &b; // Gli assegniamo l' indirizzo di una variabile char
```

Per poter far accedere questo puntatore generico al valore di una variabile andrà prima convertito al tipo di quella variabile:

```C
int a = 1;
void *generico;             // Dichiariamo il puntatore generico
generico = &a               // Gli assegniamo l' indirizzo di a
int *intero;                // Dichiariamo un secondo puntatore, di interi
intero = (int *) generico;  
```

Nella quinta riga facciamo il cast del puntatore generico da <font color="#c4bd97">void</font> a <font color="#c4bd97">int</font>, quindi assegniamo quell’indirizzo al puntatore intero.