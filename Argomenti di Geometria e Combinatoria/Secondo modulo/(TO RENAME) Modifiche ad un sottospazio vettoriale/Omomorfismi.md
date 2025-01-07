Tra le applicazioni $f:V\to W$ tra due spazi vettoriali sono particolarmente importanti gli <font color="#ffff00">Omomorfismi</font>:

Allora iniziamo a definire cosa è un omomorfismo:
Esso è un tipo particolare di funzione tra spazi vettoriali tale che valgono le seguenti proprietà:
- $f(u+v)=f(u)+f(v)$, per ogni $u\in V, \ v\in V$
- $f(ku)=kf(u)$ per ogni $k\in \mathbb{R},u\in V$

Per stabilire se una applicazione sia o meno un <font color="#ffff00">omomorfismo</font> ci sarà utile dare dei nomi alle proprietà, quindi diremo che:
- $f$ <font color="#00b050">rispetta l’ addizione</font> se soddisfa la 1° proprietà
- $f$ <font color="#00b050">rispetta la moltiplicazione</font> se soddisfa la 2° proprietà

Facciamo un banale esempio:
- Se $V$ e $W$ sono due spazi vettoriali, è facile vedere che l’ applicazione $f:V \to W$ che associa ad ogni vettore di $V$ il vettore nullo di $W$ è un <font color="#ffff00">omomorfismo</font>, esso è infatti detto <font color="#ffff00">omomorfismo nullo</font>.

Facciamo un esempio più complesso per comprendere meglio:

### <font color="#00b0f0">Esempio 1 sugli omomorfismi</font>
- Consideriamo $f:\mathbb{R^3}\to\mathbb{R}^2$ definita t.c:
$$f(x,y,z):=(x+y,y+z)$$
- Studiamo due vettori di $\mathbb{R}^3$:
  - $u:=(x_{1}+y_{1}+z_{1})$
  - $v:=(x_{2}+y_{2}+z_{2})$

- Allora verifichiamo se rispetta l’ addizione:
   $$f(u+v)=f((x_{1},y_{1},z_{1})+(x_{2},y_{2},z_{2}))$$

- Che per definizione di somma in $\mathbb{R}^3$:
$$f(x_{1}+x_{2},y_{1}+y_{2},z_{1}+z_{2})$$
- Ora applichiamo $f$:
$$(x_{1}+x_{2}+y_{1}+y_{2},y_{1}+y_{2}+z_{1}+z_{2})$$
- Quindi confermiamo che rispetti la seconda parte dell’ addizione:
$$f(u)+f(v)=f(x_{1},y_{1},z_{1})+f(x_{2},y_{2},z_{2})$$
- Applichiamo $f$:
$$(x_{1}+y_{1},y_{1}+z_{1})+(x_{2}+y_{2},y_{2}+z_{2})$$
- Ed infine per la def. di somma in $\mathbb{R}^2$:

$$(x_{1}+y_{1}+x_{2}+y_{2},y_{1}+z_{1}+y_{2}+z_{2})$$
E allora possiamo dire che la somma è rispettata.

Ora verifichiamo se rispetta anche il prodotto, prendendo in esame un vettore $u:=(x,y,z)$ ed uno scalare $k\in\mathbb{R}$
