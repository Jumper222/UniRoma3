---
tags:
  - Fondamenti_di_Informatica
---
Una <font color="#ffff00">Struct</font> in C è un tipo di variabile composta definita dal programmatore.
Esse si dicono composte perché al loro interno posso esserci più variabili, anche di tipi diversi, accessibili singolarmente, memorizzate in un unico blocco di memoria.

Si definiscono:

```C
struct Punto {  // Definiamo la struct, chiamandola Punto
	float x;    // Aggiungiamo dentro la struct una variabile float "x"
	float y;    // facciamo lo stesso, per "y"
}

struct Punto p; // definiamo una variabile di tipo Punto chiamata p.

p.x = 4,2;  // accediamo al campo x
p.y = 4.1;  // accediamo al campo y

```

è possibile passare struct come parametri di una funzione:
```C
float distanza(struct Punto p1, struct Punto p2) { // Dichiaro la funzione
	//...
}

distanza(p1,p2); // invoco la funzione
```

Per poter modificare i valori dei campi di una struct fuori da una funzione lavoriamo con [[Struct e Puntatori]]