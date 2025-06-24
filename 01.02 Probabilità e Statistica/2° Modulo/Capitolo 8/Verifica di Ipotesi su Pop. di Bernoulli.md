---
tags:
  - Probabilità_e_statistica
---
Ho un [[Campione Aleatorio]] con $n$ oggetti, dove ogni oggetto è difettoso indipendentemente dagli altri.

Come verifico le ipotesi:
- $H_{0}:p\leq p_{0}$
- $H_{1}:p>p_{0}$
*Dove p è la probabilità reale che un dato pezzo sia difettoso*

Allora svolgo come segue:

Sia $X$ il numero di pezzi difettosi nel campione

$$\mathbb{P}(X\geq k)=\sum^n_{i=k}\mathbb{P}(X=i)=\sum^n_{i=k}\binom{n}{i}p^i(1-p)^{n-1}$$
Allora cerchiamo la probabilità di avere più pezzi difettosi di un dato valore $k$.

Fissiamo un [[Livello di Significatività]] $\alpha\in(0,1)$ e quindi cerchiamo il $k$ minimo che rispetta questo livello.

$$K_{*}^\alpha=\min\left\{ k:\sum^n_{i=k}\binom{n}{i}p^i_{0}(1-p_{0})^{n-i} \right\}$$
Detto allora $x$ il numero di pezzi difettosi nel campione,
- Se $n\bar{x}<K_{*}^\alpha$ accetto $H_{0}$
- Altrimenti rifiuto.

Posso inoltre definire la [[p-value]]:

$$\sum^n_{i=n\bar{x}}\binom{n}{i}p_{0}^i(1-p_{0})^{n-i}=\mathbb{P}(X>\bar{x}n\ |\ H_{0})$$
E allora posso dire di rifiutare $H_{0}$ per ogni [[Livello di Significatività]] $\alpha>p-value$.

Facciamo un esempio:

Un produttore afferma che non più del $2\%$ degli oggetti che produce è difettoso.
Compriamo 300 pezzi e ne troviamo 10 difettosi.

Allora testiamo:
$H_{0}:p\leq 0.02$
$H_{1}:p>0.02$

Otteniamo che la [[p-value]] è:
$$\mathbb{P}(X\geq 10 \ | \ X\sim Bin(n,0,02))\approx 0.082$$
Qui usiamo 10 direttamente perché questa è la proporzione tra i difettosi e i pezzi totali, moltiplicata per i pezzi totali (quindi sono semplicemente i pezzi difettosi).

I dati allora portano ad accettare $H_{0}$ con una significatività del $5\%$ 

<font color="#f79646">ATTENZIONE</font>: Qui stiamo usando una [[p-value]] particolare apposta per le popolazioni di bernoulli, se provassimo a farlo con una normale, trasformando la bernoulli con il [[Teorema del Limite Centrale (CLT)]] arriveremmo ad una conclusione che ci farebbe rifiutare $H_{0}$.

Allora ci ricordiamo sempre che per le popolazioni di bernoulli vale la seguente legge:
$$p_{0}(1-p_{0})n>20$$
allora posso usare l’ approssimazione normale.
In questo esempio però otterremo circa $6$, che quindi porta ad imprecisioni gravi.