#Probabilità_e_statistica 
>[!Definizione] Definizione
>La funzione di Probabilità $\mathbb{P}$ è tale che:
>- $\mathbb{P}:P(\Omega)\to[0,1]$ (La probabilità di un qualsiasi elemento di $\Omega$ è definita tra 0 e 1)
>- $\Omega \supset E\to\mathbb{P}(E)$ (Se $E$ è contenuto in $\Omega$, allora ne esiste una Probabilità)

La funzione $\mathbb{P}$ verifica i seguenti assiomi:
1. $\mathbb{P}(E)\in[0,1], \quad\forall E\subset \Omega$
2. $\mathbb{P}(\Omega)=1$
3. $\forall E,F\subset \Omega$, t.c $E\cap F=\emptyset$ Allora $\mathbb{P}(E\cup F)=\mathbb{P}(E)+\mathbb{P}(F)$

Da questo 3° assioma si ha la seguente generalizzazione:
- Se $\forall E_{1},E_{2},\dots,E_{n}\subset \Omega$ tali che $E_{i}\cap E_{j}=\emptyset$, $\forall i,j\leq n$ tali che  $i\neq j$ Allora avremo che:
$$\mathbb{P}\left( \bigcup_{i=1}^n E_{i}\right)=\sum_{i=1}^n\mathbb{P}(E_{i})$$