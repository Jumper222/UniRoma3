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
<font color="#ff0000">!!!</font> *In questo caso il programma darà errore*

è da notare come la dichiarazione di un puntatore non allochi spazio per un array, in caso fosse aggiunto dopo:

```C
char stringa1[] = "ciao"; // è una stringa che alloca esattamente lo spazio di ciao
char* stringa2 = "wewe";  // è un puntatore che punta a 'wewe'

char* stringa3;           // è un semplice puntatore di char
fgets(stringa3,50,stdin); 
```

Nella 5° riga stiamo cercando di mettere 50 <font color="#c4bd97">char</font> dove punta il <font color="#c4bd97">puntatore</font>, però non sappiamo ne dove <font color="#9bbb59">punta</font>, ne cosa c’è in queste 50 celle di memoria, il programma andrà quindi in crash.

##### Definire un array usando puntatori

Come abbiamo visto in precedenza, possiamo creare un puntatore al primo elemento di un array,
E allora, se aggiungessimo $+x$ al valore del puntatore, ci sposteremmo di $x$ posizioni avanti.

```C
int array[3] = {1,3,7};
int *puntatore
puntatore = array;     // Se facessimo printf del *puntatore riceveremmo 1
*(array+2) = 4;        // Abbiamo modificato il 3° valore da 7 a 4.

```