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
void raddoppiatore(int y){
	y = y*2;
}

int main(){
	int x = 7;
}
```