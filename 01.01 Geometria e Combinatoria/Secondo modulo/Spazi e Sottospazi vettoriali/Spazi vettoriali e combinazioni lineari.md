#Geometria_e_Combinatoria 
Come abbiamo visto in [[Dipendenza ed indipendenza lineare dei vettori|precedenza]] una combinazione lineari di tutti i vettori dello spazio indipendenti fra loro è il modo per generare lo spazio stesso.

- Da questa nozione deriva che:
  se $V$ è generato dai vettori $v_{1},v_{2},\dots,v_{r}$,
  ed uno di essi è combinazione lineare degli altri, allora possiamo scartarlo ed ottenere $r-1$ vettori che generano $V$. Questo ovviamente possiamo continuare a farlo finché non si possono più scartare vettori.

Facciamo un esempio di 3 vettori linearmente dipendenti:
- $v_{1}:=(2,4,4,2),v_{2}:=(1,2,2,1) \ e \ v_{3}:=(1,2,3,3)$
  Allora possiamo dire che $1v_{1}-2v_{2}+0v_{3}=0$ <font color="#f79646">QUINDI</font> i vettori sono linearmente dipendenti.

<font color="#ff0000">NB</font>: Si noti che nella definizione di vettori linearmente dipendenti non si richiede che tutti i coefficienti siano diversi da 0, ma solo che qualcuno di essi (almeno uno) sia diverso da 0.

<font color="#ff0000">NB</font>: due vettori $v_{1}$ e $v_{2}$ sono linearmente dipendenti se e solo se uno di essi è multiplo dell’ altro.

Facciamo ora un esempio:

### <font color="#4bacc6">Esempio 1</font>:
Ci chiediamo se $v_{1}:=(1,2,1,0),v_{2}:=(2,3,0,1),v_{3}:=\left( 1, \frac{5}{2},2, -\frac{1}{2} \right)$
sono linearmente dipendenti tra loro.
Quindi scriviamo una loro combinazione lineare e poniamola = 0.
$$k_{1}(1,2,1,0)+k_{2}(2,3,0,1)+k_{3}\left( 1, \frac{5}{2},2,-\frac{1}{2} \right)=(0,0,0,0)$$
di conseguenza: $$\left( k_{1}+2k_{2}+k_{3},2k_{1}+3k_{2}+ \frac{5}{2}k_{3},k_{1}+2k_{3},k_{2}-\frac{1}{2}k_{3} \right)$$
Poi si va a risolvere il sistema associato: 
$$\begin{cases}
\phantom{2}k_{1}+2k_{2}+\phantom{\frac{5}{3}}k_{3}&=0 \\
2k_{1}+3k_{2}+\frac{5}{2}k_{3}&=0 \\
\phantom{1}k_{1}+\phantom{3k_{2}}+ \ 2k_{3}&=0 \\
\phantom{1k_{1}}+\phantom{3}k_{2}-\frac{1}{2}k_{3} &=0\end{cases}$$
La cui soluzione è $$\begin{cases}
k_{1}&=-2t \\
k_{2}&=\frac{1}{2}t \\
k_{3}&=t
\end{cases}$$
Ed essendo tutte e tre le variabili descrivibili da una sola variabile allora sono <font color="#f79646">linearmente dipendenti</font>.
