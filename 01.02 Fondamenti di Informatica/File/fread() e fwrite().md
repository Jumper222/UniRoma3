---
tags:
  - Fondamenti_di_Informatica
---
Queste due funzioni servono per leggere e scrivere dentro file binari.

```C
fread(&VARIABILE,sizeof(TIPOVARIABILE),1,fp);

fwrite(&VARIABILE,sizeof(TIPOVARIABILE),1,fp);
```

Queste due funzioni leggono (la prima) e scrivono su file. di solito si usano in un loop while per continuare a leggere/scrivere finché nel file ci sono informazioni, mettendo queste funzioni nella condizione del while.

```C
while(fread(&VARIABILE,sizeof(TIPOVARIABILE),1,fp)>0){
	arr[i]=variabile;
	i++;
}
```

esempio uguale per la scrittura.