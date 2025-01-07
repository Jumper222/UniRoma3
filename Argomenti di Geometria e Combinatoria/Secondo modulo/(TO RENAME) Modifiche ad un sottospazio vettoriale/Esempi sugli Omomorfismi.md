### <font color="#00b0f0">Esempio 1</font>
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

- Ora verifichiamo se rispetta anche il prodotto, prendendo in esame un vettore $u:=(x,y,z)$ ed uno scalare $k\in\mathbb{R}$:
$$f(ku)=f(k(x,y,z))$$
- Per la definizione di prodotto in $\mathbb{R}^3$:
$$f(kx, ky, kz)$$
- Per la definizione di $f$: 
$$(kx + ky, ky + kz)$$
- Verifichiamo la seconda parte:
$$kf(u) = kf(x, y, z)$$
- Per la definizione di $f$: 
$$k(x + y, y + z)$$
- Per la definizione di prodotto in $\mathbb{R}^2$:
$$(kx + ky, ky + kz)$$

Quindi possiamo dire che $f$ è un omomorfismo di spazi vettoriali su $\mathbb{R}$

### <font color="#00b0f0">Esempio 2</font>
Consideriamo l’ applicazione $f:M(2,2,\mathbb{R})\to M(2,2,\mathbb{R})$, definita t.c:
$$f(A):=A+^tA$$