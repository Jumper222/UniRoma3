Quando andiamo ad usare uno stimatore qualsiasi, dovremmo andare a studiare la sua efficienza, ossia quanto è puntuale la stima che stiamo dando, questa stima si ha con l’ errore quadratico medio:

<font color="#f79646">Errore Quadratico Medio</font> (<font color="#9bbb59">EQM</font>)
$$r(\hat{\theta})=var(\hat{\theta})+b(\hat{\theta})^2$$
dove $var(\hat{\theta})$ è la varianza secondo il parametro che abbiamo dato, e $b(\hat{\theta})^2$ è la funzione di bias, più l’ <font color="#9bbb59">EQM</font> è vicino a 0, più è corretta la stima.

<font color="#f79646">Funzione di Bias</font> (<font color="#9bbb59">b</font>)
$$b(\hat{\theta})=\mathbb{E}[\hat{\theta}]-\theta$$
Nel caso la <font color="#f79646">funzione di Bias</font> risultasse 0, avremmo un parametro ‘<font color="#9bbb59">Corretto</font>’.