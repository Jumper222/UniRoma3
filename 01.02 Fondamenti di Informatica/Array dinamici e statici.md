---
tags:
  - Fondamenti_di_Informatica
---
Una volta che impariamo a gestire l’[[Allocazione della memoria]], possiamo iniziare ad usare gli array dinamici, ossia array che cambiano di dimensione durante l’ esecuzione del programma.

Vediamo innanzitutto come dichiararne uno, e come cambia rispetto ad uno statico.

```C
int *array = malloc(n * sizeof(int)); // ARRAY DINAMICO

int array[n]; // ARRAY STATICO
```

Le principali differenze sono 3:
- Gli array statici rimangono in memoria fino al terminare della funzione in cui sono stati dichiarati, un array dinamico può essere deallocato quando fa comodo. <font color="#92d050">+MEMORY MANAGEMENT</font>
	- Gli array statici vengono memorizzati nello [[Stack]], metri gli array dinamici dentro l’[[Heap]], il secondo è tipicamente molto più grande del primo. +ARRAY