---
tags:
  - Probabilità_e_statistica
---

Il test di Indipendenza lo usiamo per sapere se esiste una dipendenza di un qualche tipo tra i dati studiati, Quindi prende sempre in considerazione vettori di [[Variabili Aleatorie|v.a.]]

Ci aspettiamo allora le seguenti ipotesi:
$H_{0}:\mathbb{P}(X=a)\mathbb{P}(Y=b)=\mathbb{P}(X=a,Y=b)$
$H_{1}:\text{altrimenti}$

Innanzitutto abbiamo la tabella osservata:


|     | 1         | 2         |
| --- | --------- | --------- |
| 1   | $O_{1,1}$ | $O_{1,2}$ |
| 2   | $O_{2,1}$ | $O_{2,2}$ |

Ora andiamo a crearci la tabella E (Expected, per [[Valore Atteso]]) dove ogni cella avrà il valore $E_{{i,j}}$:
$$E_{i,j}=\dfrac{(\text{tot colonna})(\text{tot riga})}{n}$$
Una volta ottenuta la tabella E, andiamo a calcolarne i valori veri (Non lasciamo in frazione) e si ottiene la [[Statistica Test]]:

$$T=\sum_{i=1}^\text{tot colonne}\sum^\text{tot righe}_{j=1}\left(\dfrac{(O_{i,j}-E_{i,j})^2}{E_{i,j}}\right)$$
Fortunatamente quando abbiamo un campione grande, T assomiglia ad una [[Chi Quadro]]:
Il che significa che una volta calcolato T usando la formula di sopra poi lo confronteremo con un valore della tabella di $\chi^2$ per capire se è un valore troppo “estremo”
$$T\approx \chi^2_{\text{tot colonne * tot righe}}$$
Questa [[Statistica Test]] la andiamo poi a confrontare con il [[Livello di Significatività]] richiesto:

Preso un $\alpha\in(0,1)$:

- Se $T\leq \chi^2_{\text{tot colonne * tot righe},\alpha}$ Accetto $H_{0}$
- Altrimenti rifiuto.

La [[p-value]] invece si calcola:

$$\mathbb{P}(\chi^2_{\text{tot colonne * tot righe},\alpha}>T)$$

