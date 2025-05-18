La funzione <font color="#ffc000">malloc()</font> ci permette di aggiungere <font color="#c0504d">byte</font> di memoria all’ [[Heap]] del programma, fa parte della libreria stdlib.h.

<font color="#ffc000">malloc()</font> restituisce un [[Puntatori Generici|puntatore generico]] all’ area di memoria creata, che quindi andrà convertito in un tipo specifico per poi essere utilizzato.

Se l’ esecuzione non dovesse andare a buon fine, (succede quando non rimane abbastanza RAM libera) <font color="#ffc000">malloc()</font> restituisce <font color="#b2a2c7">NULL</font>.
- è buona norma fare un check per <font color="#b2a2c7">NULL</font> ogni volta che si usa <font color="#ffc000">malloc()</font>,
- invocare un [[free()]] quando la memoria non ci è più utile.

Vediamo ora un esempio di <font color="#ffc000">malloc()</font>:

```C
int main(){
	int *interi = malloc(10 * sizeof(int));
	if(interi== NULL) { // FAIL CASE
		printf("Niente memoria :(");
	}
	else {
		for(int i=0; i<10; i++) {
			*(interi+i)=i+1;          // Memorizziamo interi da 1 a 10
		}
		printf("Ecco gli interi: ");
		for(int i=0; i<10; i++) {     // Li stampiamo
			printf("%d ", *(interi+i)); 
		}
		free(interi);                 // liberiamo la memoria prima allocata.
	}
}
```

- Per semplificare l’ uso di malloc(), di solito si usa come nella <font color="#4bacc6">riga 2</font>, dove andiamo a riservarci lo spazio per 10 elementi della grandezza di un <font color="#c4bd97">int</font>. 

In questo esempio stiamo assegnando al puntatore $*interi$ una memoria grande 4 x 10 byte, questa memoria non è inizializzata, conterrà quindi garbage (<font color="#4bacc6">riga 2</font>)

successivamente nella <font color="#4bacc6">riga 7</font> stiamo iterando dentro il puntatore per riempire le celle di memoria, mettendoci i numeri da 1 a 10. 

Infine nella <font color="#4bacc6">riga 11</font> stiamo iterando di nuovo per poi stampare.