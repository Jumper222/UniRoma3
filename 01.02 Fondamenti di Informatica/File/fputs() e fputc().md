fputs() ed fputc() sono funzioni molto simili, che servono per scrivere stringhe o caratteri nel file:

#### fputs()
Serve per scrivere stringhe non formattate in C

```C
	FILE *fp = fopen("scrittura.txt", "w");
	fputs("Scrivo ABC", fp);
```

##### fputc()
Serve per scrivere caratteri in C

```C
	FILE *fp = fopen("scrittura.txt","w");
	fputc("c",fp);
```