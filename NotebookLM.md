Per trovare la costante C in una funzione Densità di Probabilità (PDF), devi utilizzare la proprietà fondamentale che **l'integrale della PDF su tutto il suo dominio deve essere uguale a 1**. Questo perché la probabilità totale di tutti gli esiti possibili deve essere 1.

Ecco i passaggi generali per trovare la costante C:

1. **Imposta l'integrale della funzione PDF $f(x)$ sul suo intero dominio uguale a 1:** $\int_{-\infty}^{\infty} f(x) dx = 1$
    
2. **Sostituisci l'espressione della tua PDF $f(x)$, che conterrà la costante C, nell'integrale.**
    
3. **Calcola l'integrale.** I limiti di integrazione saranno determinati dal dominio in cui la PDF è definita. Al di fuori di questo dominio, la PDF è tipicamente zero.
    
4. **Risolvi l'equazione risultante per la costante C.**
    

Ad esempio, considerando la PDF fornita nella Lezione PROBSTAT2025 4.pdf:

$f(x) = C(4x - 2x^2)$ per $x \in (0, 2)$ $f(x) = 0$ altrimenti

Per trovare C, impostiamo l'integrale su tutto il dominio uguale a 1:

$\int_{-\infty}^{\infty} f(x) dx = \int_{0}^{2} C(4x - 2x^2) dx = 1$

Calcolando l'integrale:

$C \int_{0}^{2} (4x - 2x^2) dx = C \left[ 2x^2 - \frac{2}{3}x^3 \right]_{0}^{2} = C \left( (2(2)^2 - \frac{2}{3}(2)^3) - (2(0)^2 - \frac{2}{3}(0)^3) \right) = C \left( 8 - \frac{16}{3} \right) = C \left( \frac{24 - 16}{3} \right) = C \left( \frac{8}{3} \right)$

Ora, impostiamo questo risultato uguale a 1 e risolviamo per C:

$C \left( \frac{8}{3} \right) = 1$ $C = \frac{3}{8}$

Pertanto, il valore della costante C per questa PDF è $\frac{3}{8}$. La Lezione PROBSTAT2025 4.pdf sottolinea che se questa condizione ($\int_{-\infty}^{\infty} f(x) dx = 1$) non è soddisfatta, allora $f$ non può essere una PDF.