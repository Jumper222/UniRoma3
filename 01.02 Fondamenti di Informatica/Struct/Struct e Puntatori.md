---
tags:
  - Fondamenti_di_Informatica
---

Per poter modificare tramite una funzione ausiliaria dobbiamo passare i parametri per riferimento:

```C
struct Punto {  
	float x;    
	float y;    
}

void modificaCoordinate(struct Punto *puntaP) { // Passiamo l' indirizzo della struct
	(*puntaP).x = 1;
	(*puntaP).y = 1; 
}

int main() {
	struct Punto p;
	modificaCoordinate(&p); // Passiamo l' indirizzo di p
}
```

Esiste però un operatore per accedere 