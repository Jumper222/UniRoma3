Si definisce una Permutazione con ripetizione una Permutazione di elementi non tutti distinti tra loro,
in altre parole una permutazione con ripetizione è uno dei possibili modi per ordinare totalmente un certo numero di elementi, di cui alcuni ripetuti.

Facciamo caso di voler anagrammare la parola aab.

Quindi iniziamo con lo scegliere la prima lettera: a oppure b.
Se abbiamo scelto la a allora per la seconda scelta si avranno 2 possibilità, se è stata scelta la b allora avremo 1 possibilità.
In entrambi i casi l’ ultima lettera è ovvia.

Si hanno quindi 3 combinazioni: baa, aab e aba.

La formula che è dietro questo calcolo è:

$$\frac{3!}{2!*1!}$$ dove 3 sono gli elementi totali, 2 è il numero di elementi ripetuti del primo elemento e 1 è il numero di elementi ripetuti del secondo elemento.

Un altro esempio potrebbe essere per l’ anagramma della parola cassa:

avremmo:
- $n_{1}=1$ ovvero la lettera $c$
- $n_{2}=2$ ovvero la lettera $a$
- $n_{3}=2$ ovvero la lettera $s$

Il calcolo quindi sarà:
$$\frac{5!}{1!*2!*2!}\; ovvero \;\frac{120}{4} \; quindi \; 30$$