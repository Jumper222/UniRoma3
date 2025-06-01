---
tags:
  - Fondamenti_di_Informatica
---
Per cancellare per valore si hanno 2 step:
Prima si collega il nodo precedente al successivo a quello da cancellare, poi si dealloca la memoria usata per quel nodo.


```C
/* funzione che cancella il primo nodo con un certo valore */
void cancellaValore3(struct Nodo *head, int valore) {
    struct Nodo *butta; // appoggio per deallocazione di memoria
    int cancellato = 0; // inizialmente non ho cancellato niente

    /* controlla head->next, per vedere se è il nodo cercato: vai avanti fino
     * a che esiste un tale nodo e non hai trovato il nodo da cancellare */
    while (head->next != NULL && !cancellato) {
        if (head->next->numero == valore) {
            /* nodo cercato: devi collegare il precedente al successivo e buttare
             * il corrente */
            butta = head->next;
            head->next = butta->next;
            free(butta);
            cancellato = 1;
        } else {
            head = head->next;
        }
    }

    if (!cancellato) {
        printf("%d non e' presente nella lista\n", valore);
    }
}
```