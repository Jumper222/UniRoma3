---
tags:
  - Fondamenti_di_Informatica
---
In <font color="#4f81bd">C</font> quando andiamo a dichiarare un array, in realtà stiamo creando una variabile [[Puntatori|puntatore]] al primo elemento dell’ array, questo valore però è una costante, che quindi non può essere modificato: 

```C
int x;
int num[3] = {1,4,5};
num = &x; 
```
*In questo caso il programma darà errore*

