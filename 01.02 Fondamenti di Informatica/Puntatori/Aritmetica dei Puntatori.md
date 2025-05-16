---
tags:
  - Fondamenti_di_Informatica
---
Se provassimo ad aggiungere $+1$ ad un <font color="#c4bd97">puntatore</font> allora questo significa che stiamo muovendo l’ indirizzo in memoria di $i * 4$ nel caso di un puntatore di <font color="#c4bd97">interi</font>, ossia stiamo spostando la cella puntata del numero di byte che occupa il tipo di <font color="#c4bd97">variabile</font> del <font color="#c4bd97">puntatore</font>.

L’ utilità di questo si ha quando andiamo a lavorare con [[Puntatori ed Array]] perché spostandoci di x posizioni in memoria ci spostiamo anche di x posizioni all’ interno dell’ array.

```C
int num[3] = {1,3,7};
int *punta = num;                       // assegniamo 
printf("punta vale: %d", puntatore);    // Printa 1
printf("punta+1 vale: %d", puntatore+1);// Printa 3
```