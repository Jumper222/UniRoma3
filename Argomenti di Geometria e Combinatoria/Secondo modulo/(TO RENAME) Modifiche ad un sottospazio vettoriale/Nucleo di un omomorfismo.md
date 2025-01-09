Il <font color="#ffff00">nucleo</font> di un omomorfismo è il sottoinsieme dello spazio vettoriale di partenza la cui immagine è il <font color="#4bacc6">vettore</font> nullo.

Se $f:V\to W$ è un omomorfismo allora $f(0_{v})=0_{w}$

---

Facciamo un semplice esempio:

Sia $f:R^3\to R^2$ l’ applicazione definita da:
$f(x,y,z):=(x+y+3z,x+2y+4z-1)$

<font color="#f79646">ATTENZIONE PERÒ</font>: in questo caso $f$ non è lineare, in quanto $f(0,0,0)=(0,-1)\neq(0,0)$

----
Facciamo un altro esempio:

Sia $f:R^2\to R^2$ l’ applicazione definita da:
$f(x,y):=(xy,x)$

Questa legge rispetta la regola del nucleo: $f(0,0)=(0,0)$

<font color="#f79646">ATTENZIONE PERÒ</font>: nemmeno questo è un omomorfismo, in quanto non rispetta l’ addizione:
- $f(0,1)+f(1,0)=(0,0)+(0,1)=(0,1)$
- $f((0,1)+(1,0))=f(1,1)=(1,1)$

Da questi due esempi quindi capiamo che anche se viene rispettato il nucleo, non è detto che stiamo parlando di un’ applicazione lineare.

--- 

<font color="#ffff00">Studiati</font> i casi limite possiamo quindi iniziare a dare una definizione del nucleo, inteso come insieme:
- Chiameremo nucleo di $f$ ($ker\ f$) l’ insieme t.c: $ker\ f:=\{v\in V\  |\ f(v)=0_{w}\}$
<font color="#ffff00">Oltretutto</font> [[Dimostrazione sottospazio vettoriale del nucleo|possiamo dire]] che se $ker\ f$ di un omomorfismo $f:V\to W$ allora $ker\ f$ sarà un sottospazio vettoriale di $V$.

---

Facciamo un vero esempio del nucleo di un omomorfismo:

- Prendiamo l’ omomorfismo $f:R^5\to R^3$, definito da:
$$f(a,b,c,d,e):=(a-b+c)+(b-c+d)x+(c-d+e)x^2$$
- Possiamo quindi dire che il vettore $(a,b,c,d,e)$ appartiene a $ker\ f$ se e solo se:
$$(a-b+c)+(b-c+d)x+(c-d+e)x^2=0$$
- Quindi:
$$\begin{cases}
a - b + c&= 0 \\
\phantom{a+.} b - c + d&= 0 \\
\phantom{a\,b.\.,\,\,.} c - d + e&=0
\end{cases}$$
- Avendo però più incognite che equazioni, ci avvarremo dell’ uso dei parametri, ed il risultato finale sarà:
$$ker\ f=\{-t,-u,t-u,t,u\ |\ t\in R,u\in R  \}$$
- Ed allora, per trovare la base studieremo prima il sistema con $(1,0)$ e poi con $(0,1)$. Scopriremo quindi che la base è formata da:
$$(-1,0,1,1,0) \ e \ (0,-1,-1,0,1) $$

Altri [[Esempi sul nucleo|esempi]].