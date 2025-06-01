---
tags:
  - Fondamenti_di_Informatica
---
Andremo prima ad allocare la memoria per un nuovo nodo, scriverne i dati, poi lo collegheremo al nodo precedente e infine imposteremo il puntatore di questo nuovo nodo a <font color="#c0504d">NULL</font>.

```C
/* funzione che inserisce un nodo in coda alla lista */
void inserisciCoda3(struct Nodo *head) {
    struct Nodo *nuovoNodo;          // il nuovo nodo della lista
    nuovoNodo = malloc(sizeof(struct Nodo));  // allocazione nuovo nodo nell'heap

    /* riempi i campi del nuovo nodo */
    printf("Inserisci l'intero!\n");
    scanf("%d", &(nuovoNodo -> numero));
    printf("\n");
    nuovoNodo->next = NULL;

    /* collega il nodo al precedente: devi cercare l'ultimo nodo della lista, che potrebbe anche essere quello fittizio */
    
    while(head->next != NULL)        // l'ultimo nodo ha il campo next vuoto
        head = head->next;           // scorri di 1

    /* ora head contiene l'indirizzo dell'ultimo nodo della lista */
    head->next = nuovoNodo;
}
```