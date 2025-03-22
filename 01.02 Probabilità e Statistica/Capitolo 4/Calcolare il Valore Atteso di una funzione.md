#Probabilità_e_statistica 
Se ci viene data una $X$ come v.a. e degli $a,b\in \mathbb{R}$

Allora possiamo generalizzare con:
$$\mathbb{E}[aX+b]=a\ \mathbb{E}[X]+b$$
In queste situazioni consideriamo la funzione $g(x)=ax+b$
ed iniziamo a calcolare quella:
Infatti se $X$ è discreta:
$$\mathbb{E}[aX+b]=\sum _{x\in \mathrm{Im}(x)}g(x)p_{X}(x)=\sum _{x\in \mathrm{Im}(X)}(ax+b)P_{X}(x)=\dots=a\ \mathbb{E}[X]+b*1$$
Se invece $X$ è continua:
$$\int^\infty_{-\infty}g(x)f(x)dx=\int^\infty_{-\infty}(ax+b)f_{x}(x)dx=\dots=a\int^\infty_{-\infty }xf_{X}(x)dx+b\int^\infty_{-\infty }f_{X}(x)dx$$

