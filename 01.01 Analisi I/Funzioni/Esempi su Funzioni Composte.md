#Analisi_1 
### <font color="#ff0000">Esempio 01</font>

Si hanno due [[funzioni]] $f: X\to Y \;e\; g: V\to Z$, Allora:
$h(x):  g \circ f$ ha senso<font color="#e36c09"> SE E SOLO SE</font> $\mathrm{Im}(f) \subseteq V = Dom(g)$
Che sta a significare che può esistere una funzione h(x), composta di g su f(x) se e solo se l’ immagine di f è contenuta dentro V, e V è il dominio di g.

Si ha quindi il seguente grafico:
![[01.01 Analisi I/Funzioni/Excalidraw Funzioni/Funzioni composte|Funzioni composte]]

Questa funzione composta <font color="#ff0000">NON</font> è una composizione semplice, perché DOM(g) non è  uguale a $\mathrm{Im}(f)$

### <font color="#ff0000">Esempio 02</font>
Si hanno:
$f:\mathbb{R} \to \mathbb{R}$ e $g: [0, +\infty)\to \mathbb{R}$
$f: x \to x+1$ $g:y\to \sqrt{ y }$

La cui funzione composta sarà:
$$h(x)=g(f(x)) =\sqrt{ x+1 }$$
- Trovare Dom(h).

Per trovare il dominio di una funzione composta h dobbiamo imporre la funzione $f$ dentro al dominio di $g$In questo caso dobbiamo imporre $x+1\geq 0$ perché 0 è il minimo della funzione g.
Si ha quindi che Dom(h) =  $x+1\geq 0$
Sostanzialmente bisogna verificare  i valori di $f$ che hanno senso dentro la funzione $g$

### <font color="#ff0000">Esempio 03</font>
Si hanno:
$f(x)=\sqrt{ x} \;e \;g(x)=1-x^2$
Quindi i domani solo tali che:
dom(f) = {$x\geq 0$} e dom(g) = {$\mathbb{R}$}