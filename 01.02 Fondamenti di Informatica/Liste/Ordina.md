Usiamo il bubble sort per ordinare tutti gli elementi dentro la lista.

```C
// Scambia il contenuto informazione di due nodi
void scambia(struct Nodo* nodo1, struct Nodo* nodo2) {
    int app;
    app = nodo1->numero;
    nodo1->numero = nodo2->numero;
    nodo2->numero = app;
}

// Funzione bubble sort per ordinare la lista (solo scambio valori)
void ordinaLista(struct Nodo* head) {
    int fattoscambio = 1;
    int appoggio;
    struct Nodo* app = head;
    struct Nodo* ultimo = NULL;

    if (head == NULL) {
        printf("Niente da ordinare, la lista e' vuota!\n");
    }

    while (app != NULL && fattoscambio) {
        fattoscambio = 0;
        app = head;
        while (app->next != NULL) {
            if (app->numero > app->next->numero) {
                scambia(app, app->next);
                fattoscambio = 1;
            }
            app = app->next;
        }
    }
}
```