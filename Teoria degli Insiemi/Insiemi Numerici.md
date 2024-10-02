---
share_link: https://share.note.sx/9em8vcgd#zevjnY6vunMV2/8LmhtFwRzN9dx50qoua4RhY9t5kqc
share_updated: 2024-10-02T11:52:06+02:00
---
##### Insiemi Numerici
Esistono degli insiemi fondamentali nella Matematica, chiamati Insiemi Numerici.
Essi sono:
ℕ ={0; 1 ; 2 ; 3 ; 4 ...}
ℤ ={0; ±1; ±2; ±3 ...}
ℚ = {$0; \pm\frac{2}{4}; \pm\frac{3}{7}$}
ℝ = {$\sqrt{2}$}
ℂ = {$i$}

Per definire questi insiemi ci serviamo di alcuni <font color="#ff0000">assiomi</font>.
- Somma (+)
- Prodotto ($*$)
- $\exists$ elementi neutri, 0 ed 1, T.C. $x*1 = n; n + 0 = n$

Da questi assiomi possiamo ricavare delle proprietà:
- <font color="#ff0000">Associativa</font> $(a+b)+c = a + (b+c)$ e $(a*b)*c = a*(b*c)$
- <font color="#ff0000">Commutativa</font> $a+b = b+a$ e $a*b = b*a$
- <font color="#ff0000">Distributiva</font> $a*(b+c) = a*b + a*c$

# <font color="#4f81bd">Ordinamento</font>
Definiamo una relazione: ≤

Si hanno 3 proprietà:
- <font color="#ff0000">Dicotomia</font> $\forall a,b$ si ha a ≤ b oppure b ≤ a
- <font color="#ff0000">Riflessiva</font> $a\leq a$ $\forall a$ 
- <font color="#ff0000">Antisimmetria</font> se a ≤ b e b ≤ a allora a=b

#### <font color="#4f81bd">Proprietà sull’ ordinamento</font>
se a ≤ b allora $a+c\leq b+c$ $\forall c$ 
a ≥ b e b ≥ 0 allora $a*b \geq 0$

Definiamo un’ altra relazione: <
da questo ricaviamo due proprietà:
$a<b$ $\iff$ $a\leq b$ e $a\neq b$
$a\geq b \iff b\leq a$


![[Definizioni degli insiemi]]

### <font color="#4f81bd">Proprietà transitiva</font>
se $a\leq b$ e $b\leq c \implies a\leq c$ 
<font color="#ff0000">DIM</font>: ho $b-a\geq 0$ e $c-b \geq 0$
Allora: $a\leq (b-a) + (c-b) = c-a$ allora $a≤c$

### <font color="#4f81bd">Densità di Q</font>

$$\forall x,y\in \mathbb{Q},x<y \implies \exists \;\infty\; z\in \mathbb{Q} \text{ t.c } x<z<y \implies z=\frac{y-x}{z}$$
Esiste almeno un <font color="#ff0000">numero z</font> tra qualsiasi dato numero x, y all’ interno dell’ insieme Q.

### <font color="#4f81bd">Proprietà Archimede</font> 
$$\forall x,y\in\mathbb{Q}\;allora \;x,y>0 \;\exists \;n\in\mathbb{N}:n*x>y$$
Per ogni <font color="#ff0000">coppia di naturali</font> esiste un numero n che moltiplicato per x supera y

### <font color="#4f81bd">Assioma di Completezza</font>

Dati A $\subseteq$ $\mathbb{R}$ e B $\subseteq \mathbb{R}$ sottoinsiemi,
t.c. che $a\leq b\; \forall a \in A \; \land \; \forall b \in B$
$\exists$ almeno un numero reale $c\in \mathbb{R} \text{ t.c. } a\leq c\leq b \; \forall a\in A \; \land \; \forall b\in B$
- L' <font color="#ff0000">Assioma</font> afferma che ogni insieme non vuoto di numeri Reali ha sempre un limite superiore (numero più grande). questo significa che non ci sono vuoti nei numeri reali.
- In altre parole non è possibile avere un insieme di numeri reali che non raggiunge il suo limite in <font color="#ff0000">R</font>


### <font color="#4f81bd"> Modi di descrivere un insieme</font>
(Argomento di Geometria e Combinatoria)


Si hanno 2  modi per descrivere un insieme:

$A=$ {2;4;6;8}
B = {$x\in\mathbb{N} \;| \;1\leq x\leq 9 \; \land x \; pari$}

Questi due insiemi sono uguali, però sono definiti in modo diverso