Per verificare se due variabili aleatorie congiunte, diciamo X e Y, sono indipendenti tra loro, si possono utilizzare diverse definizioni e proprietà, a seconda che le variabili siano discrete o continue.

**Definizione Generale di Indipendenza:** Due variabili aleatorie X e Y si dicono **indipendenti** se per ogni coppia di insiemi A appartenente all'immagine di X (Im(X)) e B appartenente all'immagine di Y (Im(Y)), si verifica che: **P(X ∈ A, Y ∈ B) = P(X ∈ A)P(Y ∈ B)**. Questa condizione significa che la probabilità che X assuma un valore in A e contemporaneamente Y assuma un valore in B è uguale al prodotto delle probabilità individuali di questi eventi.

**Condizioni per Variabili Aleatorie Discrete:** Se X e Y sono variabili aleatorie discrete con funzione di massa di probabilità congiunta P_{X,Y}(x, y) e funzioni di massa di probabilità marginali P_X(x) e P_Y(y) rispettivamente, allora X e Y sono indipendenti se e solo se: **P_{X,Y}(x, y) = P_X(x) P_Y(y)** per ogni x ∈ Im(X) e y ∈ Im(Y). In pratica, per verificare l'indipendenza, si calcolano le PMF marginali da quella congiunta (sommando sulle righe o sulle colonne della tabella di probabilità congiunta) e poi si verifica se il prodotto delle marginali è uguale alla congiunta per tutte le coppie (x, y).

**Condizioni per Variabili Aleatorie Continue:** Se X e Y sono variabili aleatorie continue con funzione di densità congiunta f_{X,Y}(x, y) e funzioni di densità marginali f_X(x) e f_Y(y) rispettivamente, allora X e Y sono indipendenti se e solo se: **f_{X,Y}(x, y) = f_X(x) f_Y(y)** per ogni x ∈ ℝ e y ∈ ℝ. Per verificare l'indipendenza, si calcolano le PDF marginali integrando la PDF congiunta rispetto all'altra variabile e poi si verifica se il prodotto delle marginali è uguale alla congiunta per tutte le coppie (x, y).

**Altre Proprietà Equivalenti per l'Indipendenza:**

- **Funzioni di Ripartizione (CDF):** X e Y sono indipendenti se e solo se la loro funzione di ripartizione congiunta F_{X,Y}(x, y) è uguale al prodotto delle loro funzioni di ripartizione marginali: **F_{X,Y}(x, y) = F_X(x) F_Y(y)** per ogni x ∈ ℝ e y ∈ ℝ. Dove F_{X,Y}(x, y) = P(X ≤ x, Y ≤ y), F_X(x) = P(X ≤ x), e F_Y(y) = P(Y ≤ y).
    
- **Valore Atteso:** Se X e Y sono indipendenti, allora il valore atteso del loro prodotto è uguale al prodotto dei loro valori attesi: **E[XY] = E[X]E[Y]**. Più in generale, se X e Y sono indipendenti, allora per qualsiasi coppia di funzioni g e h tali che E[g(X)] e E[h(Y)] esistano, si ha: **E[g(X)h(Y)] = E[g(X)]E[h(Y)]**. **Attenzione:** Il viceversa non è sempre vero, ovvero E[XY] = E[X]E[Y] non implica necessariamente l'indipendenza di X e Y.
    
- **Funzione Generatrice dei Momenti (MGF):** Se X e Y sono indipendenti, allora la funzione generatrice dei momenti della loro somma è il prodotto delle loro MGF individuali: **P_{X+Y}(t) = P_X(t)P_Y(t)** per ogni t per cui le MGF sono definite. Equivalentemente, la MGF congiunta di X e Y, P_{X,Y}(t_1, t_2) = E[e^{t_1X + t_2Y}], è il prodotto delle MGF marginali: **P_{X,Y}(t_1, t_2) = P_X(t_1)P_Y(t_2)**.
    

In sintesi, per verificare l'indipendenza, la strategia principale è quella di confrontare la distribuzione congiunta (PMF o PDF) con il prodotto delle distribuzioni marginali. Le altre proprietà possono essere utili in alcuni contesti, ma la definizione basata sulle distribuzioni è la più fondamentale.