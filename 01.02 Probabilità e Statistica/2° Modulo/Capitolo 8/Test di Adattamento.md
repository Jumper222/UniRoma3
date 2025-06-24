---
tags:
  - Probabilità_e_statistica
---
Facciamo un esempio:

![[Test di Adattamento ESEMPIO.png]]

Abbiamo un campione $Y_{1}\dots Y_{n}\in\{-6,-5\dots5\}$ *12 categorie*

Chiamo $X_{-6}\dots X_{5}$ quante $Y$ valgono $i$:
$$X_{i}=\sum^n_{j=1}\mathbb{1}(Y_{j}=i)$$

Allora per testare l’ affermazione qui sopra creo le ipotesi:
$H_{0}:\mathbb{P}(Y=i)=\dfrac{1}{12}$
$H_{1}:\mathbb{P}(Y=i)\neq \dfrac{1}{12}$
*Per un qualche $i$ compreso tra -6 e 5*

Allora per individuare la [[Statistica Test]] procedo come segue:

$$T=\sum^5_{i=-6}$$