---
tags:
  - Fondamenti_di_Informatica
---
La funzione <font color="#ffc000">fscanf()</font> in C è usata per leggere sequenze di caratteri da un file.
Prende in input vari parametri:
1. è il puntatore al file che vogliamo leggere
2. è la stringa che ci dice il formato dei caratteri che vogliamo leggere (<font color="#92d050">%d</font>,<font color="#92d050">%c</font>, ecc)
3. Ogni parametro successivo indica gli indirizzi delle variabili a cui vogliamo assegnare i valori letti.

Un esempio d’uso:

```C
FILE *fp = fopen("scrittura.txt, "r");
char carattere;
int intero;
fscanf(fp, "%c%d", &carattere, &intero); 
```

