---
tags:
  - Fondamenti_di_Informatica
---

La funzione <font color="#f79646">calloc()</font> è stretta parente di [[malloc()]], appartiene alla libreria stdlib.h, e ci permette di allocare una parte di memoria all’ [[Heap]] del programma, inizializzando tutti gli indirizzi a 0.
In input <font color="#f79646">calloc()</font> prende due parametri: il numero di elementi da allocare nell’ [[Heap]], e la loro dimensione.

potremmo vedere <font color="#f79646">calloc()</font> come un’ alternativa più “elegante” di [[malloc()]], in quanto non ci sarà bisogno di inventarci strane moltiplicazioni con <font color="#f79646">sizeof()</font> per poter gestire più elementi.

esattamente come [[malloc()]], <font color="#f79646">calloc()</font> ci restituisce un [[Puntatori Generici|puntatore generico]] che poi andrà convertito, e in caso non basti la RAM restituirà NULL.

Essendo quasi uguale a [[malloc()]], vediamo come due dichiarazioni con uguale risultato differiscono.

```C
int main(){
	int *interi = malloc(10 * sizeof(int));
	int *interi = calloc(10,sizeof(int));
}
```

come possiamo vedere la principale differenza sta nel fatto che non dobbiamo far eseguire al programma 