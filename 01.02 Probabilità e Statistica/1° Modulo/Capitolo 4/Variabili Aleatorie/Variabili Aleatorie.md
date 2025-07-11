---
tags:
  - Probabilità_e_statistica
aliases:
  - v.a.
  - V.a.
---


> [!Definizione]  Definizione
> Descriviamo un [[Modello Probabilistico]] per il nostro esperimento aleatorio:
> La variabile aleatoria è una [[Funzioni|funzione]] ($X$) che prende in input $(\Omega,\mathbb{P})$ (ossia un singolo evento e la sua probabilità) così che possiamo specificare la probabilità dei singoli [[Eventi]] possibili.
> 

Facciamo un esempio con i dadi:

Lanciamo 2 dadi.
Abbiamo lo spazio campionario $\Omega$ che rappresenta tutte le possibili coppie:
$\Omega:\{(1,1),(1,2),\dots,(6,6)\}$

Ora supponiamo che la variabile aleatoria $X$ sia la somma dei due dadi:
$$X(a,b)=a+b$$
Quindi avremo:
- Se esce (2,5) allora $X=7$
- Se esce (3,3) allora $X=6$

Allora questa funzione trasforma gli esiti casuali in numeri reali, permettendoci di calcolare la probabilità di ottenere certi valori (es: “Quanto è probabile ottenere un 7”)

---

Ora facciamo un esempio più pratico:
Acquisto 2 componenti elettronici, essi possono essere:
- <font color="#00b050">Accettabili</font> (prob. 0,7)
- <font color="#f79646">Difettosi</font> (prob. 0,3)

Quindi avremo $\Omega=\{(a,a),(a,d),(d,a),(d,d)\}$
Iniziamo a calcolare le probabilità:
$\mathbb{P}(a,a)=0,7*0,7=0,49$
$\mathbb{P}(d,d)=0,3*0,3=0,09$
$\mathbb{P}(a,d)=\mathbb{P}(d,a)=0,7*0,3=0,21$

Allora chiamo $X$ il numero di componenti accettabili, quindi il numero di valori che $X$ può assumere saranno {0,1,2}

$\mathbb{P}(X=0)=\mathbb{P}(d,d)=0,09$
$\mathbb{P}(X=1)=\mathbb{P}\{(a,d),(d,a)\}=2*0,21=0,42$
$\mathbb{P}(X=2)=\mathbb{P}(a,a)=0,49$

Oppure chiamo $I$ la variabile aleatori che vale:
- $1$: Se ha almeno un componente accettabile
- $0$: altrimenti

Queste variabili che hanno $\mathrm{Im}=\{0,1\}$ sono chiamate [[Variabili Aleatorie Indicatrici]]
E allora $\mathbb{P}(I=0)=\mathbb{P}(X=0)=0,09$ e $\mathbb{P}(I=1)=\mathbb{P}(X\geq1)=0,91$

Le variabili aleatorie ci portano ad avere la [[Fun. di Ripartizione (CDF)]]

Allora abbiamo la [[Fun. di massa di Probabilità (PMF)]]

Inoltre ci sono le [[Coppie e vettori di variabili aleatorie]]

Esattamente come gli [[Eventi indipendenti]], esistono le [[Variabili Aleatorie Indipendenti|variabili aleatorie indipendenti]]

Quindi abbiamo anche il concetto di [[Valore Atteso]] 