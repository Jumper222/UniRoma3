---
tags:
  - Fondamenti_di_Informatica
---
Quando passiamo dei valori in una funzione esistono 2 metodi, per valore e per riferimento

##### Passaggio parametri per valore

Quando passiamo dei <font color="#9bbb59">parametri</font> per valore stiamo passando dei valori attuali attraverso una <font color="#ffc000">funzione</font>, questi valori poi vengono assegnati a variabili all’ interno della <font color="#ffc000">funzione</font>, diventando <font color="#9bbb59">parametri</font> formali.
Le modifiche ai <font color="#9bbb59">parametri</font> formali non hanno effetto sui <font color="#9bbb59">parametri</font> attuali.

Un esempio:
```C
int raddoppiatore(int y){
	return y*2;
}

int main(){
	int x = 7;
	x = raddoppiatore(x);
	printf("Ecco il doppio di 7: %d",x);
}
```


##### Passaggio parametri per riferimento

Quando passiamo dei <font color="#9bbb59">parametri</font> per riferimento stiamo passando direttamente le <font color="#4bacc6">aree di memoria</font>, ossia i [[Puntatori]] delle variabili, cosi che un effetto all’ interno della <font color="#f79646">funzione</font> agisca anche all’ infuori.

```C
void raddoppiatore(int *x){
	*x = *x *2;
}

int main(){
	int x = 7;
	raddoppiatore(&x);
	printf("Ecco il doppio di 7: %d",x);
}
```

