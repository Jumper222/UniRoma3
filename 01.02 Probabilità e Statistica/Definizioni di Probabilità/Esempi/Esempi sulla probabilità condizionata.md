#Probabilità_e_statistica 
### <font color="#4bacc6">Esempio 1</font>:

Lancio 2 dadi, uno rosso ed uno blu, allora:
$|\Omega|=6*6=36$ 
Supponiamo che gli eventi siano equiprobabili, Consideriamo l’ evento $E$:

$E$: “La somma dei dadi da 8”=$\{(2,6),(3,5),(4,4),(5,3),(6,2)\}$
Abbiamo quindi che $\mathbb{P}(E)=\frac{5}{36}$

Ora  consideriamo un evento $F$: 

$F$: “Il dado rosso da 3” = $\{(3,1),(3,2),(3,3),(3,4),(3,5),(3,6)$

Quanto vale $\mathbb{P}(E)$ se so che $F$ si verifica?

Varrà $\frac{1}{6}$, che deriva dalla formula iniziale.

---

### <font color="#4bacc6">Esempio 2</font>:

In una scatola ho $40$ componenti elettroniche
- $5$ guaste (non funzionano)
- $10$ difettose (funzionano per $1h$ e poi si rompono)
- $25$ accettabili (funzionano)

Allora scelgo una componente a caso:
- $G$: è guasta
- $D$: è difettosa
- $A$: è accettabile

$\mathbb{P}(G)=\frac{5}{40}$
$\mathbb{P}(D)=\frac{10}{40}$
$\mathbb{P}(A)=\frac{25}{40}$

Ora supponiamo che inizialmente la componente funzioni → $D\cup A=G^c$
Quale sarà la probabilità di $A$?

Sarà tale che: $$\mathbb{P}(A|G^c)=\frac{\mathbb{P}(A\cap G^c)}{\mathbb{P}(G^c)}=\frac{\mathbb{P}(A\cap(D\cup A))}{1-\mathbb{P}(G)}=\frac{\mathbb{P}(A)}{1-\mathbb{P}(G)}=\frac{\frac{25}{40}}{1-\frac{5}{40}}=\frac{25}{35}$$
In questi casi il nuovo spazio campionario si indica con $\widetilde{\Omega}$, quindi abbiamo che $|\widetilde{\Omega}|=35$
Lo spazio rimane equiprobabile, perciò: $$\widetilde{\mathbb{P}}(A)=\frac{25}{25+10}=\frac{25}{35}$$

### <font color="#4bacc6">Esempio 3</font>:

Un signore ha 2 figli/e
ciascuno dei due figli/e ha $50\%$ probabilità di essere M e $50\%$ di essere F.
$\Omega=\{(M,M),(F,M),(M,F),(F,F)\}$
Ora supponiamo di aver incontrato uno dei figli, e che esso sia M.
Quale è la probabilità che anche l’ altro sia M?

So che $A$: “Almeno uno dei figli è M” si è verificato

Allora: $$\mathbb{P}(\{(M,M)\}|A)=\frac{\mathbb{P}(\{(M,M)\}\cap A)}{\mathbb{P}(A)}=\frac{|\{(M,M)\}|}{|\{(M,M),(M,F),(F,M)\}|}=\frac{1}{3}$$
Supponiamo allora di sapere che il figlio che abbiamo incontrato sia il primogenito, Allora:
$$\mathbb{P}(\{M,M\}|B)=\frac{\mathbb{P}(\{(M,M)\}\cap B)}{\mathbb{P}(B)}=\frac{1}{2}$$
