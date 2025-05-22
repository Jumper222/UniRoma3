---
tags:
  - Probabilità_e_statistica
---
Il metodo di [[Stima Parametrica]] usando gli Stimatori Bayesani si basa sull’ effettuare una stima per $\theta$, conoscendo oltre alla distribuzione, anche delle informazioni a priori su come è distribuito, chiamata $\pi(\theta)$.


> [!definizione]  Definizione
> Dati un [[Campione Aleatorio]] $(x_{1},\dots,x_{n})$ di [[Variabili Aleatorie|v.a.]] [[IID]], una funzione [[Fun. di densità di Probabilità (PDF)|PDF]] o [[Fun. di massa di Probabilità (PMF)|PMF]] $f(x\ |\ \theta)$ ed una informazione a priori su $\theta$ (come è distribuito) che chiamiamo $\pi(\theta)$
> Per ottenere la distribuzione a posteriori calcoliamo:
> $$\left(\prod^n_{i=1}f(x_{i}|\theta)\right)\pi(\theta)$$
> Questa distribuzione, per $n\gg 0$ si avvicina sempre di più al parametro.
> Però questa rimane una distribuzione, ed invece a noi serve un numero.
> Dovremmo quindi applicare una <font color="#9bbb59">Loss Function</font>, ossia una funzione che data una distribuzione ci ritorna un valore.
> Le 2 <font color="#9bbb59">Loss Function</font> più importanti sono:
> - <font color="#4f81bd">Quadratica</font>:
>	Cerco la media della distribuzione a posteriori, è quella che si usa la maggior parte delle volte.
>	$$\hat{\theta}_{bayes}=\int \theta \left(\prod^n_{i=1}f(x_{i}|\theta)\right)\pi(\theta)$$
>- <font color="#4f81bd">Linex(c)</font> (<font color="#9bbb59">Linear Exponential</font>):
>	è utile se vogliamo una stima più conservativa, infatti tenderà ad essere sempre sotto la media di $\theta$, prende in input un parametro $c>0$.
>	$$-\dfrac{1}{c}lg\ \mathbb{E}[e^{-cY}]$$
>	Dove $Y$ è la distribuzione a posteriori.
>	

