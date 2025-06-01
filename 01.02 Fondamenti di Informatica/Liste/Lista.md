---
tags:
  - Fondamenti_di_Informatica
---
Una Lista è una particolare struttura di dato dove le  informazioni sono contenute in <font color="#9bbb59">NODI</font>, ognuno dei quali ha il proprio dato memorizzato ed il [[Puntatori|puntatore]] al nodo successivo.
La creazione e distruzione di questi nodi avviene tramite [[malloc()]] e [[free()]], permettendo quindi una gestione della memoria più efficiente di quel che fa un array.

L’ ultimo <font color="#9bbb59">nodo</font> di una lista ha il [[Puntatori|puntatore]] che punta a <font color="#c0504d">NULL</font>, per segnare la fine della lista.
Nello [[Stack]] per accedere alla lista usiamo la <font color="#9bbb59">head</font> o testa, che è una variabile [[Puntatori|puntatore]] che punta al primo <font color="#9bbb59">nodo</font>.

Un esempio per un nodo potrebbe essere:

```C
typedef struct Nodo {
	int numero;
	NODO *next;
}NODO;
```

Una particolarità delle liste è che per accedere al nodo in coda bisogna prima accedere a tutti gli altri nodi, infatti le operazioni sulla coda sono sempre meno efficienti di quelle che agiscono sulla testa.


Per gestire le liste esistono varie funzioni:

- [[Visualizzazione di una Lista]]
- [[Inserimento in testa]]
- [[Inserimento in coda]]
- [[Cancellazione primo elemento]]
- [[Cancellazione per valore]]
- [[Trova il Massimo]]