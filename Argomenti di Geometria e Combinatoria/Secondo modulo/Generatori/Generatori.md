Un insieme di <font color="#ffff00">generatori</font> è un insieme grazie al cui ogni vettore di uno spazio vettoriale può essere descritto come combinazione lineare dei vettori contenuti nel sistema.

Il concetto di <font color="#ffff00">generatore</font> è intimamente collegato al concetto di combinazione lineare dei singoli vettori.

Nello specifico:
- L’ insieme $L$ delle combinazioni lineari dei vettori $v_{1},v_{2},\dots,v_{r}$ al variare dei coefficienti $k_{1},k_{2},\dots,k_{r}$       è un sottospazio vettoriale di $V$ chiamato sottospazio vettoriale <font color="#ffff00">generato</font> dai vettori $v_{1},v_{2},\dots,v_{r}$
  <font color="#ff0000">NB</font>: tale sottospazio vettoriale contiene i vettori $v_{1},v_{2},\dots,v_{r}$ ed è contenuto in <font color="#ff0000">tutti</font> i sottospazi vettoriali di $V$ contenenti $v_{1},v_{2},\dots,v_{r}$.

Facciamo un esempio generalizzato della definizione per capire meglio il concetto.
### <font color="#4bacc6">Esempio 1 di un generatore</font>

- Abbiamo l’ insieme $L(v_{1},v_{2},\dots v_{r})$
  Notiamo subito che $L$ contiene tutti i vettori $v_{1},v_{2},\dots v_{r}$
  Ad <font color="#ffff00">esempio</font> $v_{1}=1v_{1}+0v_{2}+\dots+0v_{r}$
  Allora definiamo $E$ come un sottospazio vettoriale di $V$ contenente $v_{1},v_{2},\dots v_{r}$
  Allora per definizione di un sottospazio vettoriale possiamo anche dire che $E$ contiene anche               tutti i vettori del tipo $k_{1}v_{1},k_{2}v_{2},\dots,k_{r},v_{r}$
  Allora di conseguenza $E$ contiene anche tutte le combinazioni lineari del tipo $k_{1}v_{1}+k_{2}v_{2}+\dots+k_{r}v_{r}$
  **<font color="#f79646">QUINDI</font> possiamo dire che $E$ è generato da $L(v_{1},v_{2},\dots, v_{r})$

  In altre parole, essendo $E = L(v_{1},v_{2},\dots,v_{r})$ allora $E$ è <font color="#ffff00">generato</font> dai vettori $v_{1},v_{2},\dots,v_{r}$
  E quindi abbiamo anche il rapporto inverso:
  $v_{1},v_{2},\dots, v_{r}$ sono generatori di $E$ (dato se e solo se ogni vettori di $E$ è comb. lineare di $v_{1},v_{2},\dots,v_{r}$ )

### <font color="#4bacc6">Esempio 2 di un generatore</font>

- Data una retta $r$ passante per l’ origine $O$ del piano, e dato un punto $A$ della retta $r$ distinto da $O$,
  l’insieme dei <font color="#e36c09">vettori</font> $\overrightarrow{OP}$ con $P$ giacente su $r$ è un sottospazio vettoriale <font color="#ffff00">generato</font> dal vettore $\overrightarrow{OA}$
  Possiamo quindi dire che dati in $V^2(O)$ due <font color="#e36c09">vettori</font> $\overrightarrow{OP}_{1}$ e $\overrightarrow{OP}_{2}$ con $O$, $P_{1}$ e $P_{2}$ non allineati, i <font color="#e36c09">vettori</font> $\overrightarrow{OP}_{1}$ e $\overrightarrow{OP}_{2}$ <font color="#ffff00">generano</font> $V^2(O)$.

