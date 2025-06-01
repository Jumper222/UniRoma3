---
tags:
  - Fondamenti_di_Informatica
---
A livello teorico quel che andiamo a fare è creare una nuovo nodo, a cui linkeremo il nodo subito dopo l’ head, poi modificheremo il puntatore dell’ head per puntare al nuovo nodo.

```C
typedef struct Nodo {
	int numero;
	struct Nodo next;
}NODO;

NODO *inserisci Nodo(NODO *head) {
	NODO nuovoNodo;
	nuovoNodo = malloc(sizeof(NODO);
										// leggi il campo dati
	printf("Inserisci l'intero!\n");
	scanf("%d", &(nuovoNodo -> numero));
										// collega il nodo al successivo
	nuovoNodo->next = head;
									// restituisci l'indirizzo del nuovo primo elemento
	return nuovoNodo;
}
   // Dentro al main:
Nodo(head);
```
