---
tags:
  - Fondamenti_di_Informatica
---
Per poter visualizzare una [[Lista]], passiamo dentro la funzione direttamente il puntatore della <font color="#9bbb59">head</font>, e poi gli diciamo di iterare con un while la lista, andando ogni volta al nodo successivo. il while si fermerà quando abbiamo che il puntatore è <font color="#c0504d">NULL</font>

```C
void stampa(NODO *head) {
	NODO *nodo = head;
	if (nodo == NULL) {
	printf("Lista vuota")    //lista vuota
	}
	else {
		while(nodo!=NULL) {
			printf("%d ", nodo->numero);
			nodo = nodo -> next;
		}
	}
}
```