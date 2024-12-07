#Analisi_1
il principio di Induzione è un fondamentale passo logico utile in matematica per generalizzare tesi che sono vere per più valori, senza doverne calcolare ogni valore.

Sostanzialmente, si realizza considerando una proprietà vera per $n$ e controllandone la verità per n+1

Il principio si divide in vari step:

Si considera una proprietà o affermazione, indicizzata da un indice $n\in \mathbb{R}\to P_{n}$
Si suppone quindi che $P_{n}$ sia vera per $n=1$
Quindi si controlla che $P_{n}$ sia vera per $n+1$ 
Allora si ha una verità per tutto $\mathbb{N}$

Possiamo prendere per esempio la Serie di Gauss, ovvero la somma dei primi $n$ numeri naturali.

$$\sum_{k=1}^{n} k = \frac{n(n+1)}{2}$$

Iniziamo quindi a controllare se per 1 il ragionamento ha senso:

$$1=\frac{1*(1+1)}{2}=1$$
In questo esempio il primo 1 è detto “base di induzione”

Si ha quindi il passo induttivo:

$$\sum_{k=1}^{n+1} k = \frac{(n+1)(n+2)}{2}$$
Ovvero si prova ad usare $n+1$ al posto di $n$
