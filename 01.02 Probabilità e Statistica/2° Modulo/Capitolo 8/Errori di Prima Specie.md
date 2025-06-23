---
tags:
  - Probabilità_e_statistica
---
Negli esercizi di errore di prima specie ci viene richiesto, data una ipotesi nulla ed una alternativa, se accettare o rifiutare la nulla.

Vediamo il procedimento:

#### <font color="#4bacc6">ERRORI PRIMA SPECIE</font> ($\alpha$)

0. $H_{0}:\mu=\mu_{0}$ oppure $H_{1}:\mu\neq m_{0}$
	*L’ ipotesi Nulla $H_{0}$ è vera oppure è falsa?

1.  Fisso un [[Livello di Significatività]] $\alpha\in(0,1)$
	*Ossia fisso un valore per il quale voglio che la statistica che ho ottenuto dai campioni si avvicini a* $H_{0}$.

2. Calcolo la [[p-value e Statistica Test|Statistica Test]]:
 $$\dfrac{\sqrt{ n }}{\sigma}|\bar{x}-\mu|$$
	 *La statistica test è una funzione dell’ insieme dei dati, che allora li rappresenta.*

3. Calcolo la probabilità che la statistica assuma il valore dello step 2:
$$\mathbb{P}(\ |Z|>\dfrac{\sqrt{ n }}{\sigma}|\bar{x}-\mu|\ )=p-value$$
- <font color="#f79646">Attenzione</font>:
	1. Avendo il valore assoluto di Z, bisogna ricordarsi di levarlo e moltiplicare per 2 la probabilità
	2. Accetterò $H_{0}$ se la <font color="#9bbb59">p-value</font> è maggiore o uguale ad $\alpha$, altrimenti rifiuto
	3. Nella pratica non si fissa un valore $\alpha$, ma si riporta solo il <font color="#9bbb59">p-value</font>

