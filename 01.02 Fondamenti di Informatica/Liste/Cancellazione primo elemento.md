---
tags:
  - Fondamenti_di_Informatica
---
Per quanto riguarda la cancellazione del primo elemento i passaggi saranno prima modificare la testa della lista, mettendoci l’ indirizzo del secondo nodo, poi libereremo la memoria usata per il precedente primo nodo:

```C
/* funzione che cancella un nodo dalla testa della lista */
void cancellaNodo3(struct Nodo *head) {
    struct Nodo *app;  // il nuovo primo nodo della lista

    /* lista vuota? */
    if (head->next != NULL) {
        app = head->next;  // memorizzo l'indirizzo del nodo da cancellare per deallocarlo
        head->next = app->next;
        free(app);
    }
}
```