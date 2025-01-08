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