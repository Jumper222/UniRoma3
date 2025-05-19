Il Typedef è un modo per dare un alias, ed è molto usata per le struct:

```C
typedef struct Punto {
	float x;
	float y;
} PUNTO;

int main() {
	PUNTO p1;
}
```