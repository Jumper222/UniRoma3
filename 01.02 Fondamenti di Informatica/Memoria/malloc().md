La funzione <font color="#ffc000">malloc()</font> ci permette di aggiungere <font color="#c0504d">byte</font> di memoria all’ [[Heap]] del programma.

<font color="#ffc000">malloc()</font> restituisce un [[Puntatori Generici|puntatore generico]] all’ area di memoria creata, che quindi andrà convertito in un tipo specifico per poi essere utilizzato.

Se l’ esecuzione non dovesse andare a buon fine, (succede quando non rimane abbastanza RAM libera) <font color="#ffc000">malloc()</font> restituisce NULL.
- è buo