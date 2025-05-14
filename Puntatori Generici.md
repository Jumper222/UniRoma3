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
Generico = &a; // Gli assegniamo il valore di una variabile intera
Generico = &b; // Gli assegniamo il valore di una variabile char
```

