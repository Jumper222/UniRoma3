#Geometria_e_Combinatoria
L’ Algebra  Booleana è un ramo della matematica dove le variabili possono assumere solo i valori 0 ed 1 ( Vero o Falso.)

L’ <font color="#f79646">Algebra Booleana</font> prende in esame solo le proposizioni t.c. possano avere una risposta logica VERO/FALSO.

Ad esempio <font color="#ff0000">NON SONO</font>  proposizioni:
- x<1
- Che ore sono?
- Tutti i giorni d’ estate piove almeno 2 ore

<font color="#00b050">SONO</font> invece proposizioni:
- Londra è una citta d’ Europa
- 1+1 = 4
- Madrid è la capitale d’ Italia

Sono fondamentali in questa branca gli **Operatori Logici** <font color="#ff0000">AND</font>, <font color="#ff0000">OR</font>, <font color="#ff0000">NOT</font>

### <font color="#4f81bd">AND</font>
L’ Operatore Logico <font color="#4f81bd">AND</font> ($\land$) è un operatore con 2 input e un output, la cui tabella di verità è t.c:
<font color="#ff0000">N.B</font>: L’ operazione di doppia implicazione ($\iff$) che indica il caso di SE e solo SE, ha una tabella di verità uguale all’ AND.

| <center>P</center> | <center>Q</center> | P$\land$Q          |
| ------------------ | ------------------ | ------------------ |
| <center>1</center> | <center>1</center> | <center>1</center> |
| <center>1</center> | <center>0</center> | <center>0</center> |
| <center>0</center> | <center>1</center> | <center>0</center> |
| <center>0</center> | <center>0</center> | <center>0</center> |

### <font color="#4f81bd">OR</font>
L’ Operatore Logico <font color="#4f81bd">OR</font> ($\lor$) è un operatore con 2 input ed un output, la cui tabella di verità è t.c:

| <center>P</center> | <center>Q</center> | P$\lor$Q           |
| ------------------ | ------------------ | ------------------ |
| <center>1</center> | <center>1</center> | <center>1</center> |
| <center>1</center> | <center>0</center> | <center>1</center> |
| <center>0</center> | <center>1</center> | <center>1</center> |
| <center>0</center> | <center>0</center> | <center>0</center> |

### <font color="#4f81bd">NOT</font>
L’ Operatore Logico <font color="#4f81bd">NOT</font> ($\lnot$) è un operatore con un input ed un output, la cui tabella di verità è t.c:

| <center>P</center> | $\lnot$P           |
| ------------------ | ------------------ |
| <center>1</center> | <center>0</center> |
| <center>0</center> | <center>1</center> |

### <font color="#4f81bd">IMPLICAZIONE</font>
L’ Operatore logico della Implicazione ($\implies$) è un operatore con 2 input ed un output, la cui tabella di verità è t.c:

| <center>P</center> | <center>Q</center> | P$\implies$Q       |
| ------------------ | ------------------ | ------------------ |
| <center>1</center> | <center>1</center> | <center>1</center> |
| <center>1</center> | <center>0</center> | <center>0</center> |
| <center>0</center> | <center>1</center> | <center>1</center> |
| <center>0</center> | <center>0</center> | <center>1</center> |

### <font color="#4f81bd">TAUTOLOGIA E CONTRADDIZIONE</font>
Non sono operatori logici, piuttosto proprietà di una data operazione logica,
<font color="#f79646">Tautologia</font> è usata per indicare una proposizione sempre vera,
<font color="#f79646">Contraddizione</font> è usata per indicare una proposizione sempre falsa.