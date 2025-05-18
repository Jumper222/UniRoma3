La funzione <font color="#ffc000">malloc()</font> ci permette di aggiungere <font color="#c0504d">byte</font> di memoria all’ [[Heap]] del programma, fa parte della libreria stdlib.h.

<font color="#ffc000">malloc()</font> restituisce un [[Puntatori Generici|puntatore generico]] all’ area di memoria creata, che quindi andrà convertito in un tipo specifico per poi essere utilizzato.

Se l’ esecuzione non dovesse andare a buon fine, (succede quando non rimane abbastanza RAM libera) <font color="#ffc000">malloc()</font> restituisce <font color="#b2a2c7">NULL</font>.
- è buona norma fare un check per <font color="#b2a2c7">NULL</font> ogni volta che si usa <font color="#ffc000">malloc()</font>.

Vediamo ora un esempio di <font color="#ffc000">malloc()</font>:

```C
int main(){
	int *interi = malloc(10*sizeof(int));
	if(interi== NULL) { // FAIL CASE
		printf("Niente memoria :(");
	}
	else {
		for(int i=0; i<10; i++) {
			*(interi+i)=i+1;       //
		}
		printf("Ecco gli interi: ");
		for(int i=0; i<10; i++) {
			printf("%d ", *(interi+i));
		}
		free(interi);
	}
}
```
