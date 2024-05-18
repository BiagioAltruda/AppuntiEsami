---
aliases:
  - monotona
  - monotone
---
Sia $A\subset\mathbb{R}$ e $f:A\to\mathbb{R}$, si dice che $f$ è 
1. crescente se: $$\forall x,y\in A,\,[x<y\Rightarrow f(x)<f(y)]$$
2. debolmente crescente se: $$\forall x,y\in A,\,[x<y\Rightarrow f(x)\leq f(y)]$$
3. debolmente decrescente se: $$\forall x,y\in A,\,[x<y\Rightarrow f(x)\geq f(y)]$$
4. decrescente se: $$\forall x,y\in A,\,[x>y\Rightarrow f(x)<f(y)]$$
Se $f$ soddisfa una delle quattro proprietà precedenti, si dice che è *monotona*.
Le funzioni crescenti conservano l'ordine, mentre quelle decrescenti lo invertono.

---
*Proposizione*:
1. Somma di funzioni crescenti è crescente;
2. somma di funzioni decrescenti è decrescente;
3. composizione di funzioni monotone è monotona, il tipo di monotonia dipende dalla crescenza o decrescenza delle funzioni.

---
*Proposizione*:
Una funzione strettamente monotona è iniettiva.
*Dimostrazione*:
Dimostriamo il caso $f$ crescente, l'altro è analogo.
Comunque presi due punti distinti $x,y$, uno è minore dell'altro, supponiamo $x<y$, allora $f(x)<f(y)$ in particolare sono valori diversi. dunque $f$ è iniettiva $\blacksquare$ 
*Proposizione*:
Una funzione $f:A\subset\mathbb{R}\to\mathbb{R}$ è monotona e invertibile allora $f^{-1}$ ha lo stesso tipo di monotonia.
#funzioni 
