---
tags:
  - Fondamenti_di_Informatica
---
Una volta che impariamo a gestire l’[[Allocazione della memoria]], possiamo iniziare ad usare gli array <font color="#76923c">dinamici</font>, ossia array che cambiano di dimensione durante il runtime.

Vediamo innanzitutto come dichiararne uno, e come cambia rispetto ad uno <font color="#d99694">statico</font>.

```C
int *array = malloc(n * sizeof(int)); // ARRAY DINAMICO

int array[n]; // ARRAY STATICO
```

Le principali differenze sono 3:
- Gli array <font color="#d99694">statici</font> rimangono in memoria fino al terminare della funzione in cui sono stati dichiarati, un array <font color="#76923c">dinamico</font> può essere deallocato quando fa comodo. <font color="#92d050">+GESTIONE DELLA MEMORIA</font>
- Gli array <font color="#d99694">statici</font> vengono memorizzati nello [[Stack]], mentre gli array <font color="#76923c">dinamici</font> dentro l’[[Heap]], il secondo è tipicamente molto più grande del primo. <font color="#92d050">+GRANDEZZA ARRAY</font>
- Mentre la dimensione degli array <font color="#d99694">statici</font> è fissa, gli array <font color="#76923c">dinamici</font> hanno una dimensione che può essere modificata durante il runtime.