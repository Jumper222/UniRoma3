---
tags:
  - Fondamenti_di_Informatica
---
Una <font color="#ffff00">Struct</font> in C è un tipo di variabile composta definita dal programmatore.
Esse si dicono composte perché al loro interno posso esserci più variabili, anche di tipi diversi, accessibili singolarmente, memorizzate in un unico blocco di memoria.

Si definiscono:

```C
struct Punto {  // Definiamo la struct, chiamandola Punto
	float x; 
	float y; 
}

struct Punto p;
```