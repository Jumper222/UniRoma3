Le funzioni <font color="#ffc000">fgets()</font> e <font color="#ffc000">fgetc()</font> sono funzioni per ottenere stringhe o caratteri da un <font color="#9bbb59">file</font>, 


##### fgets()

Prende in input 3 parametri:
1. Il primo parametro è un puntatore alla variabile in cui verrà memorizzata la stringa
2. Il secondo parametro $n$ è il numero massimo di caratteri da leggere +1
3. Il terzo parametro è il puntatore al <font color="#9bbb59">file</font>

La funzione interrompe la lettura quando si raggiunge la end of line, o fine <font color="#9bbb59">file</font>

```C
FILE *fp = fopen("scrittura.txt, "r");
char buffer[20];
fgets(buffer, 20, fp);
```

##### fgetc()

prende in input il puntatore al <font color="#9bbb59">file</font> dal qualche vogliamo leggere un <font color="#4f81bd">char</font>, restituisce il carattere letto.

```C
FILE *fp = fopen("scrittura.txt, "r");
char c;
c = fgetc(fp);
```