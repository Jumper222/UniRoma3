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

Nella 5° riga quel che stiamo facendo è prima convertire il valore di <font color="#4bacc6">generico</font> (l’ <font color="#9bbb59">indirizzo</font> di <font color="#4bacc6">a</font>) in un puntatore intero, poi lo stiamo trasferendo dentro intero.