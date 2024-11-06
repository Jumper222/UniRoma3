Si dice Coefficiente Binomiale il numero naturale definito a partire da una coppia di numeri naturali, solitamente n e k, ed intende il numero di sottoinsiemi con k elementi che si possono estrarre da un insieme di n elementi.

La cui notazione è: $$\binom{n}{k}$$
<font color="#ff0000">NB</font>: Si sottintende che l’ ordine degli elementi in questi sottoinsiemi non sia rilevante, e che gli elementi dei sottoinsiemi debbano essere distinti tra loro

Volessimo fare un esempio pratico:

$\binom{4}{2}$ è il numero di sottoinsiemi di k=2 elementi che si possono comporre da un insieme che contiene n=4 elementi.
Quindi con un insieme A= {a,b,c,d} si avranno 6 sottoinsiemi totali:
{a,b} ; {a,c} ; {a,d} ; {b,c} ; {b,d} ; {c,d}

Quindi abbiamo $\binom{4}{2}$ = 6.


In questo esempio calcolare il numero di sottoinsiemi risulta facile, però per numeri più grandi potrebbe non essere così semplice, ci viene in aiuto infatti la formula del <font color="#ffff00">Calcolo del coefficiente binomiale</font>

Abbiamo quindi:

$$\binom{n}{k}=\frac{n!}{k!(n-k)!}$$
Oppure, se n < k il Coeff. Binomiale restituirà 0 per definizione.

<font color="#ff0000">NB</font>: il Coeff. Binomiale fornisce il numero di combinazioni semplici di n elementi distinti presi k alla volta.