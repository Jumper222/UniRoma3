---
tags:
  - Fondamenti_di_Informatica
---
Se provassimo ad aggiungere $+1$ ad un <font color="#c4bd97">puntatore</font> allora questo significa che stiamo muovendo l’ indirizzo in memoria di $i * 4$ nel caso di un puntatore di <font color="#c4bd97">interi</font>, ossia stiamo spostando la cella puntata del numero di byte che occupa il tipo di <font color="#c4bd97">variabile</font> del <font color="#c4bd97">puntatore</font>.

L’ utilità di questo si ha quando andiamo a lavorare con [[Puntatori ed Array]] perché spostandoci di x posizioni in memoria ci spostiamo anche di x posizioni all’ interno dell’ array.

```C
int num[3] = {1,3,7};
int *punta = num;                        // Assegniamo a punta il primo indirizzo
printf("punta vale: %d", puntatore);     // Printa 1
printf("punta+1 vale: %d", puntatore+1); // Printa 3
```

In questo caso se poniamo che il primo elemento del puntatore risiede a <font color="#8064a2">0x2236</font>, allora nella 4° riga staremo puntando:
$punta+1=2236+(1*4)=2240$
