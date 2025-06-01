---
tags:
  - Fondamenti_di_Informatica
---
Per trovare il massimo semplicemente iteriamo all’ interno della lista, aggiornando ogni volta il valore massimo quando ne troviamo uno maggiore, in modo simile a come faremmo con un array.

```C
/* relazione d'ordine fra due nodi, restituisce 1 se il primo è maggiore del secondo */
int maggiore(struct Nodo *nodo1, struct Nodo *nodo2) {
    int risultato;
    if ((nodo1->numero) > (nodo2->numero))
        risultato = 1;
    else
        risultato = 0;
    return risultato;
}

/* calcola elemento massimo nella lista */
struct Nodo* massimo(struct Nodo *head) {
    // pre: almeno un nodo nella lista
    struct Nodo *massimo = head;       // inizialmente il massimo è il primo nodo
    struct Nodo *nodo = head->next;    // parti dal secondo nodo
    /* vai avanti fino a che ci sono elementi */
    while (nodo != NULL) {
        if (maggiore(nodo, massimo))
            massimo = nodo;
        nodo = nodo->next;
    }
    return massimo;
}
```