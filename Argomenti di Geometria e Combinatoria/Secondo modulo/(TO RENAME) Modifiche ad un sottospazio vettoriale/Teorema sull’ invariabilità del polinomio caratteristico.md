Al variare della base il polinomio caratteristico di un endomorfismo non cambia.

> [!enunciato]
  Sia $f:V\to V$ un endomorfismo di uno spazio vettoriale $V$ di dim. finita.
  Sia $A$ la matrice rappresentativa di $f$ rispetto ad una base di $V$.
  Sia $A'$ la matrice rappresentativa di $f$ rispetto ad una seconda base di $V$.
  Avremo quindi che $\det(A'-\lambda I)=\det(A-\lambda I)$

---
> [!dimostrazione]
> $\det(A'-\lambda I)=\det(M^{-1}AM-\lambda I)$ ………………..…………..………..per via di ($A'=M^{-1}AM$)
> $\det(M^{-1}AM-\lambda I)=\det(M^{-1}AM-M^{-1}(\lambda I)M)$ ………...….per via di ($I=M^{-1}IM$)
> $\det(M^{-1}AM-M^{-1}(\lambda I)M)=\det(M^{-1}(A-\lambda I)M)$ ………per via della prop. delle matrici
> $\det(M^{-1}(A-\lambda I)M)=\det M^{-1}\det(A-\lambda I)\det M$ …….....per via di $\det(AB)=\det A \det B$
> $\det M^{-1}\det(A-\lambda I)\det M=\det(A-\lambda I)$ …………………..per via di $\det M^{-1}=(\det M)^{-1}$

