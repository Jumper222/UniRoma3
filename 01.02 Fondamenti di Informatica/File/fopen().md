---
tags:
  - Fondamenti_di_Informatica
---
La funzione <font color="#ffc000">fopen()</font> in C serve per aprire file, prende in input 2 parametri, il nome del file, e la modalità con cui aprirlo, restituisce un puntatore all’ interno del file, oppure <font color="#d99694">NULL</font> nel caso l’ operazione non sia andata a buon fine.

La sintassi è: 
```C
FILE *fp = fopen("File.txt","w");
```

##### Tipi di operazione

- “<font color="#f79646">r</font>” apertura in sola lettura, restituisce <font color="#d99694">NULL</font> se il file non esiste
- “<font color="#f79646">w</font>” apertura in sola lettura, crea un file con quel nome (sovrascrive se già esiste)
- “<font color="#f79646">r+</font>” apertura in lettura e scrittura, restituisce <font color="#d99694">NULL</font> se il file non esiste
- “<font color="#f79646">w+</font>” apertura in lettura e scrittura, crea un file con quel nome (sovrascrive se già esiste)
- “<font color="#f79646">a</font>” apertura in scrittura alla fine del file, crea un file con quel nome (sovrascrive se già esiste)
- “<font color="#f79646">a+</font>” apertura in lettura e scrittura, se il file non esiste viene creato (sovrascrive se già esiste)
- “<font color="#f79646">b</font>” si aggiunge ad una delle modalità di sopra per aprire un file binario

Anche per fopen() è buona norma fare un check per <font color="#d99694">NULL</font> per assicurarsi che sia andato a buon fine.