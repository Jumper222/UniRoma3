---
tags:
  - Fondamenti_di_Informatica
---
La funzione fopen() in C serve per aprire file di testo, prende in input 2 parametri, il nome del file, e la modalità con cui aprirlo, restituisce un puntatore all’ interno del file, oppure <font color="#d99694">NULL</font> nel caso l’ operazione non sia andata a buon fine.

La sintassi è: 
```C
FILE *fp = fopen("File.txt","w");
```

