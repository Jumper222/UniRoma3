---
tags:
  - Fondamenti_di_Informatica
---

<font color="#f79646">realloc()</font> fa parte della stessa famiglia di funzioni di [[malloc()]] e [[calloc()]], anch’essa appartiene a stdlib.h
Prende in input 2 valori: il puntatore da modificare e la nuova dimensione.
<font color="#f79646">realloc()</font> non inizializza la memoria che sta allocando, allora essa conterrà garbage.

Quel che realloc() ci permette di fare è modificare la quantità di memoria occupata da un puntatore gestito da [[malloc()]] o [[calloc()]] in precedenza.

Il suo utilizzo è molto semplice, facciamo un esempio con [[calloc()]]:

```C
int main() {
	int *punta = calloc(10, sizeof(int));
	// eseguiamo codice, non ci bastano più 10 int...
	punta = realloc(punta,40*sizeof(int));
}
```

