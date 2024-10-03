#Analisi_1 
### <font color="#4f81bd">Iniettiva</font>
Una funzione $f: X\to Y$ si dice <font color="#f79646">Iniettiva</font> solo se elementi <font color="#ffff00">distinti</font> del dominio hanno immagini <font color="#ffff00">distinte</font>
Ha tali <font color="#ffff00">definizioni</font> equivalenti:
- $\forall( x_{1},x_{2}) \in X: x_{1}\neq x_{2} \implies f(x_{1})\neq f(x_{2})$
- $\forall(x_{1},x_{2})\; se \; f(x_{1})=f(x_{2}) \implies x_{1} =x_{2}$
- $\forall y\in im(f)\;\exists! x \in X: f^{-1}(\{y\})=\{x\}$
![[Funzione Iniettiva]]
### <font color="#4f81bd">Suriettiva</font>
Una funzione $f:X\to Y$ si dice <font color="#f79646">Suriettiva</font> solo se <font color="#ffff00">ogni</font> elemento del $COD(f)$ è immagine di un <font color="#ffff00">qualche</font> elemento del $DOM(f)$
Ha tali <font color="#ffff00">definizioni</font> equivalenti:
- $\forall  y\in Y \;\exists x\in X:f(x)=y$
- $im(f)=f(x)=y$
- $f^{-1}({y}) \neq \emptyset \; \forall y\in Y$
![[Funzione Suriettiva]]

### <font color="#4f81bd">Biettiva</font>
Una funzione $f:X\to Y$ è <font color="#f79646">Biettiva</font> se è sia <font color="#f79646">Uniettiva</font> che <font color="#f79646">Suriettiva</font>
Ed è <font color="#ffff00">definita</font> t.c:
$$\forall y\in Y\;\exists! x:f(x)=y$$
Esempio di funzione Biettiva:

![[Funzione Biettiva]]


<font color="#ff0000">NB</font>: 
- **Iniettiva**: Se tracci delle **rette orizzontali** sul grafico della funzione e una retta interseca il grafico in **più di un punto**, allora la funzione **non è iniettiva**. Per essere iniettiva, **ogni retta orizzontale deve intersecare al massimo un punto**.

- **Suriettiva**: Se tracci delle **rette orizzontali** e una retta **non interseca** mai il grafico della funzione (ossia, passa in una zona del codominio dove la funzione non ha valori), allora la funzione **non è suriettiva**. Per essere suriettiva, **ogni retta orizzontale** deve intersecare il grafico **almeno in un punto**.

<font color="#ff0000">NB</font>:
- Una funzione potrebbe non essere Iniettiva o Suriettiva se definita in $\mathbb{R}$, ma lo può diventare se ristretta in un certo range di valori, ad esempio la funzione $y=x^2$ è suriettiva se limitata per
	$COD(f)$ = $\mathbb{R_{+}}$ 