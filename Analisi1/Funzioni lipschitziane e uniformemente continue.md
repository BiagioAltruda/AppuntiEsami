Una funzione reale $f$ si dice lipschitziana se esiste una costante $L\geq 0$ tale che:
$$
\forall x,y\in \text{dom}f,\quad |f(x)-f(y)|\leq L|x-y|
$$
$f$ si dice $L$-lipschitziana.

---
*Proposizione 6.39*:
Ogni funzione lipschitziana è continua.
*Dimostrazione*:
Basta osserva che se $f$ è $L$-lipschitziana e $|x-x_{*}|<\frac{\varepsilon}{L}$ si ha
$$
|f(x)-f(x_{*})|\leq L|x-x_{*}|<L \frac{\varepsilon}{L}=\varepsilon. \quad\blacksquare
$$
---
Una funzione $f$ si dice uniformemente continua se
$$
\forall \varepsilon > 0, \exists\delta>0: \forall x,y\in \text{dom}f, \quad |x-y|<\delta \Rightarrow |f(x)-f(y)|<\varepsilon
$$

*Proposizione 6.40*:
Una funzione uniformemente continua è continua.

---
*Teorema 6.41*(Heine-Cantor):

---
#funzioni 