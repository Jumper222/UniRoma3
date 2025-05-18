La funzione <font color="#f79646">free()</font> serve per deallocare memoria, ossia rendere della memoria dentro l’ [[Heap]] di un programma di nuovo libera.

Per farlo bisogna semplicemente dargli in input il puntatore creato precedentemente da [[malloc()]] o [[calloc()]].

<font color="#f79646">free()</font> andrebbe invocata ogni volta che l’ uso della memoria gestita da [[malloc()]] o [[calloc()]] è finito.

Allora si potrebbe usare:

```C
int main(){
	int *interi = calloc(10,sizeof(int));
	// eseguiamo codice ecc...
	free(interi);
}
```