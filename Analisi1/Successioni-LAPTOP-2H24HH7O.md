1. Si dice *successione* una qualunque applicazione definita in una semiretta di $\mathbb{N}$
2. Si dice *sottosuccessione* (o estratta) di una successione $\{a_n\}_n$ la composizione $a\,\circ\,k$, dove $k:\mathbb{N}\to\mathbb{N}$ è una qualunque applicazione crescente.

---
*Proposizione*:
Sia $\{a_n\}_n$ una successione, se $\exists M\in\mathbb{R}$ tale che definitivamente $a_n\leq M$ allora la successione $\{a_n\}_n$ è *limitata superiormente*.
*Dimostrazione*:
Sia $a_n\leq M$ per $n\geq \bar{n}$, Posto $A=\{a_0,\dots, a_{n-1},M\}\neq\emptyset$, ha un numero finito di elementi, infatti ce ne sono $\bar{n}+1$. Posto $M'=\max A$, $M'\geq M$, perché $M\in A$ e vale anche:
$$0\leq n \leq \bar{n}-1 \Rightarrow a_n\in A \Rightarrow a_n\leq M'$$
$$n\geq\bar{n}\Rightarrow a_n\leq M\Rightarrow a_n\leq M'$$
In ogni caso la successione è limitata superiormente. $\blacksquare$

---

[[Limite]] di successioni.

---
*Proposizione*:
Una successione $\{a_n\}_n$ è infinitesima se e solo se la successione dei valori assoluti è infinitesima.
[[Teoremi di confronto per successioni]]
#SuccessionieSerie