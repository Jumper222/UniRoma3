Il **Processo di Poisson** è un modello matematico utilizzato in probabilità per descrivere il verificarsi di **eventi casuali e indipendenti nel tempo (o nello spazio) ad un tasso medio costante**. È considerato la versione "continua" del processo di Bernoulli.

**A cosa serve in dettaglio?**

1. **Modellare eventi che accadono casualmente nel tempo o nello spazio**: Il processo di Poisson è particolarmente utile quando si analizzano fenomeni in cui gli eventi si verificano in modo apparentemente casuale, senza una precisa regolarità. L'attenzione non è tanto sul momento esatto in cui un evento si verifica, quanto sul numero di eventi che si verificano in un dato intervallo di tempo o regione di spazio.
    
2. **Quantificare la probabilità del numero di eventi**: La proprietà fondamentale del processo di Poisson è che il **numero di eventi che si verificano in un intervallo di tempo (o spazio) di lunghezza $t-s$ segue una distribuzione di Poisson con parametro $\lambda(t-s)$**, dove $\lambda$ è l'intensità o tasso del processo. Questo significa che possiamo calcolare la probabilità di osservare esattamente $k$ eventi in quell'intervallo usando la formula della distribuzione di Poisson:
    
    $P(N(t) - N(s) = k) = \dfrac{e^{-\lambda(t-s)} (\lambda(t-s))^k}{k!}$
    
    Dove $N(t)$ rappresenta il numero di eventi fino al tempo $t$.
    
3. **Analizzare i tempi di inter-arrivo**: Un'altra caratteristica importante del processo di Poisson è che **i tempi tra un evento e il successivo (tempi di inter-arrivo) seguono una distribuzione Esponenziale con parametro $\lambda$**. Se $X_k$ è il tempo tra l'$(k-1)$-esimo e il $k$-esimo arrivo, allora $X_k \sim Exp(\lambda)$. Questa proprietà è cruciale per analizzare la frequenza con cui gli eventi si susseguono.
    
4. **Sfruttare la proprietà di assenza di memoria**: Poiché i tempi di inter-arrivo sono distribuiti esponenzialmente, il processo di Poisson gode della **proprietà di assenza di memoria**. Questo significa che la probabilità che un evento si verifichi in futuro non dipende da quanto tempo è trascorso dall'ultimo evento. Ad esempio, se stiamo modellando il guasto di una macchina con un processo di Poisson, la probabilità che si guasti nel prossimo intervallo di tempo è la stessa indipendentemente da quanto tempo ha funzionato finora.
    
5. **Modellare l'arrivo di richieste o elementi**: Il processo di Poisson è ampiamente utilizzato per modellare l'arrivo di clienti in una coda, messaggi (email, Whatsapp), chiamate telefoniche, guasti di macchinari, o in generale l'occorrenza di eventi puntuali in un continuum.
    
6. **Approssimare la distribuzione Binomiale per eventi rari**: Come indicato nella fonte, la distribuzione di Poisson può essere usata come **approssimazione della distribuzione Binomiale quando il numero di prove $n$ è molto grande e la probabilità di successo $p$ è molto piccola**, mantenendo il prodotto $\lambda = np$ costante e di ordine 1. Questo è utile per modellare il numero di volte in cui si verifica un evento raro in un gran numero di tentativi.
    
7. **Gode di proprietà di chiusura rispetto alla somma**: Se abbiamo due processi di Poisson indipendenti con intensità $\lambda_1$ e $\lambda_2$, il **processo risultante dalla somma dei due (cioè il conteggio totale degli eventi) è ancora un processo di Poisson con intensità $\lambda_1 + \lambda_2$**. Questa proprietà di "riproducibilità" è molto utile nell'analisi di sistemi complessi.
    

**Esempi di applicazione tratti dalle fonti:**

- Il numero di messaggi Whatsapp, email o chiamate ricevute in un certo intervallo di tempo può essere modellizzato come un processo di Poisson.
- La probabilità che si verifichino un certo numero di incidenti in una settimana su un tratto autostradale, dato un tasso medio, può essere calcolata usando un processo di Poisson.
- Il processo di Poisson può essere utilizzato per studiare quante volte si viene disturbati mediamente durante un periodo di studio, considerando diverse fonti di disturbo (Whatsapp, email, chiamate).
- Il tempo di inter-arrivo degli eventi in un processo di Poisson segue una distribuzione Esponenziale, come la durata di una batteria o il tempo tra i guasti di un macchinario.

In sintesi, il **processo di Poisson è uno strumento fondamentale per modellare e analizzare fenomeni probabilistici in cui eventi si verificano in modo casuale e indipendente a un tasso medio costante nel tempo o nello spazio**. Permette di calcolare la probabilità del numero di eventi in un dato intervallo, analizzare i tempi tra gli eventi e sfruttare importanti proprietà come l'assenza di memoria e la chiusura rispetto alla somma per risolvere una vasta gamma di problemi pratici.