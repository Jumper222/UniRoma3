#Geometria_e_Combinatoria 
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
$$f(A) = A + A^t.$$
Verifichiamo la somma: $$\begin{align}
f(A+B) &= A + B + (A+B)^t \\
&= A + B + A^t + B^t, \\
f(A) + f(B) &= A + A^t + B + B^t.
\end{align}$$
Quindi $f$ rispetta la somma. Ora verifichiamo la moltiplicazione:
$$\begin{align}
f(kA) &= kA + (kA)^t \\
&= kA + kA^t, \\
kf(A) &= k(A + A^t) \\
&= kA + kA^t.
\end{align}$$
Quindi abbiamo che $f$ rispetta entrambe le proprietà, allora è un omomorfismo.

### <font color="#00b0f0">Esempio 3</font>

Consideriamo l’ applicazione $f:\mathbb{R}^2\to\mathbb{R}^2$, definita t.c:
$$f(x,y)=(x^2,x+y)$$
Quindi verifichiamo che $f$ sia un omomorfismo, per verificare l’ addizione consideriamo i vettori $u:=(x_{1},y_{1})$ e $v:=(x_{2},y_{2})$:
$$\begin{align}
f(u+v) &= f((x_1, y_1) + (x_2, y_2)) \\
&= f(x_1+x_2, y_1+y_2) \\
&= ((x_1+x_2)^2, x_1+x_2+y_1+y_2) \\
&= (x_1^2 + 2x_1x_2 + x_2^2, x_1+x_2+y_1+y_2), \\
f(u) + f(v) &= f(x_1, y_1) + f(x_2, y_2) \\
&= (x_1^2, x_1+y_1) + (x_2^2, x_2+y_2) \\
&= (x_1^2 + x_2^2, x_1+x_2+y_1+y_2).
\end{align}$$
In questo caso possiamo notare che la relazione non è sempre verificata, basta considerare i vettori $u:=(1,0)$ e $v:=(1,0)$ dunque $f$ non è un omomorfismo.