---
tags:
  - Fondamenti_di_Informatica
---
Ci permette di scrivere sequenze di caratteri in un <font color="#9bbb59">file</font>, prende in input il puntatore al <font color="#9bbb59">file</font> e la stringa da scrivere. 
restituisce il numero di caratteri scritti.

```C
FILE *fp = fopen("scrittura.txt", "w");
	fprintf(fp, "Espresso macchiato");
```

