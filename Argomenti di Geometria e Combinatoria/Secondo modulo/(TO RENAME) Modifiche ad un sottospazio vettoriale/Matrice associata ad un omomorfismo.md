Supponiamo di avere un omomorfismo $f:V\to W$ di spazi vettoriali. Se conosciamo l’ <font color="#f79646">immagine</font> di due vettori $u$ e $v$ tramite $f$ allora ovviamente conosciamo anche l’ immagine di $u+v$.
Inoltre possiamo determinare la anche l’ <font color="#f79646">immagine</font> di vettori del tipo $ku$.

Ѐ quindi utile chiedersi: se conosciamo l’ <font color="#f79646">immagine</font> $f$ di un distinto numero di vettori, di quali altri vettori possiamo determinare l’ <font color="#f79646">immagine</font>? Per saperlo basta seguire il seguente utile ragionamento:

Proposizione 

Sia $f:V\to W$ un omomorfismo di spazi vettoriali. Siano $v_{1},v_{2},\dots,v_{n}$ vettori di $V$ e $k_{1},k_{2},\dots,k_{n}$
scalari. Si ha:

$$f(k_{1}v_{1}+k_{2}v_{2}+\dots+k_{n}v_{n})=k_{1}f(v_{1})+k_{2}f(v_{2})+\dots+k_{n}f(v_{n})$$

Si evince subito quindi che conoscendo $f(v_{1}),f(v_{2}),\dots,f(v_{n})$ potremmo calcolare l’ immagine di tutti i vettori che sono comb. lineare di $v_{1},v_{2},\dots,v_{n}$.


### <font color="#9bbb59">Proposizione e dimostrazione di f=g</font>

Enunciamo e dimostriamo la seguente proposizione:

- Siano $f:V\to W$ e $g:V\to W$ due omomorfismi di spazi vettoriali. avremo quindi che se $v_{1},v_{2},\dots,v_{n}$ generano $V$ e $f(v_{j})=g(v_{J})$ per $1\leq j\leq n$ allora $f=g$ 

Dimostriamo quindi che $f(v)=g(v)$ per ogni vettore $v\in V$

Sappiamo che $v$ è descrivibile come comb. lineare di $v_{1},v_{2},\dots,v_{n}$:
$v=k_{1}v_{1}+k_{2}v_{2}+\dots+k_{n}v_{n}$

Allora possiamo espandere la proposizione appena enunciata:

$$\begin{align}
f(v) = f(k_1v_1 + k_2v_2 + ... + k_nv_n) = k_1f(v_1) + k_2f(v_2) + ... + k_nf(v_n) \\
g(v) = g(k_1v_1 + k_2v_2 + ... + k_nv_n) = k_1g(v_1) + k_2g(v_2) + ... + k_ng(v_n)
\end{align}$$
Quindi, poiché $f(v_{1})=g(v_{1}),\dots,f(v_{n})=g(v_{n})$ potremo dire che $f(v)=g(v)$
