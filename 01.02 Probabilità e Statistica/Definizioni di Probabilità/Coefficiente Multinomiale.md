#Probabilità_e_statistica 
Il <font color="#ffff00">Coefficiente Multinomiale</font> è una generalizzazione del [[Coefficiente Binomiale]]:
>[!Definizione]  Definizione
>Dato un insieme di $n$ oggetti divisi in $k\leq n$ gruppi, con
>$n_{1}$ nel gruppo 1
>$\dots$
>$n_{k}$ nel gruppo $k$
>Allora possiamo dire che ci sono:
>$$\binom{n}{n_{1},\dots,n_{k}}=\frac{n!}{n_{1}!,\dots,n_{k}!}$$
>possibili ordinamenti degli $n$ oggetti se gli elementi di ciascun gruppo sono indistinguibili tra loro.

Facciamo qualche esempio:
Supponiamo che a Sanremo, con 29 posti disponibili, ci siano:
- <font color="#ffff00">11</font> uomini
- <font color="#ffff00">10</font> donne
- <font color="#ffff00">8</font> gruppi
Allora quale è la possibilità che nella top 5 ci siano 2 uomini, 2 donne ed 1 gruppo? (assumendo che gli esiti siano equiparabili!)

Allora avremo che l’ evento $E$ sarà tale che:
$$|E|=\binom{11}{2}\binom{10}{2}\binom{8}{1}$$
E invece $\Omega$:
$$|\Omega|=\binom{29}{5}$$
Quindi il risultato finale sarà:
$$\mathbb{P}(E)=\frac{\binom{11}{2}\binom{10}{2}\binom{8}{1}}{\binom{29}{5}}$$
---

Facciamo un secondo esempio:

In un campionato di 20 squadre:

- Ne stanno $8$ del nord $(n_{1}\dots n_{8})$
- Ne stanno $5$ del centro $(c_{1}\dots c_{5})$
- Ne stanno $7$ del sud $(s_{1}\dots s_{7})$

Supponendo che le varie squadre siano indistinguibili tra loro, quanti sono gli esiti possibili per la classifica di campionato?

$20!$ classifiche possibili (se distinguiamo le squadre)
però ci sono:
- $8!$ modi per ordinare le squadre del nord
- $5!$ modi per ordinare le squadre del centro
- $7!$ modi per ordinare le squadre del sud

Allora: $$|\Omega|=\frac{20!}{8!5!7!}$$