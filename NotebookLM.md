Per calcolare la **varianza di una variabile indicatrice**, possiamo seguire questi passaggi basandoci sulle informazioni presenti nelle fonti:

- **Definizione di variabile indicatrice:** Una variabile indicatrice $I$ di un evento $E$ è una variabile aleatoria che assume solo due valori:
    
    - 1 se l'evento $E$ si verifica.
    - 0 se l'evento $E$ non si verifica. L'insieme dei valori che $I$ può assumere è $Im(I) = {0, 1}$.
- **Probabilità associate:** La probabilità che la variabile indicatrice assuma il valore 1 è la probabilità dell'evento $E$, ovvero $P(I=1) = P(E)$. La probabilità che assuma il valore 0 è la probabilità del complemento di $E$, ovvero $P(I=0) = P(E^c) = 1 - P(E)$.
    
- **Valore atteso:** Il valore atteso di una variabile indicatrice $I$ è dato da: $E[I] = 0 \cdot P(I=0) + 1 \cdot P(I=1) = P(E)$.
    
- **Calcolo di $E[I^2]$:** Per calcolare la varianza, abbiamo bisogno anche di $E[I^2]$. Poiché $I$ può assumere solo i valori 0 e 1, $I^2$ può anch'esso assumere solo i valori $0^2 = 0$ e $1^2 = 1$. Quindi, $I^2 = I$. Pertanto, il valore atteso di $I^2$ è lo stesso del valore atteso di $I$: $E[I^2] = 0^2 \cdot P(I=0) + 1^2 \cdot P(I=1) = 0 \cdot (1 - P(E)) + 1 \cdot P(E) = P(E)$.
    
- **Formula della varianza:** La varianza di una variabile aleatoria $X$ è definita come $Var(X) = E[X^2] - (E[X])^2$. Applicando questa formula alla variabile indicatrice $I$, otteniamo: $Var(I) = E[I^2] - (E[I])^2 = P(E) - (P(E))^2 = P(E) (1 - P(E))$.
    

Quindi, la **varianza di una variabile indicatrice dell'evento $E$ è $P(E)(1 - P(E))$**, che è anche uguale a $P(E)P(E^c)$.