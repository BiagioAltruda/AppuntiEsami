Diciamo che la successione $\{a_n\}_n$ ammette *limite* $l\in\bar{\mathbb{R}}$ (i numeri reali estesi) o più brevemente, tende ad $l$, se:
$$\forall U\in\mathcal{F}_l,\,\exists\bar{n}\in\mathbb{N}:\forall n\geq\bar{n},\quad a_n\in U$$
in tal caso scriviamo $a_n\to l$

---
*Teorema*:
Il limite di una successione, se esiste, è unico.
*Dimostrazione*:
se $a_n\to l_1$ e $a_n\to l_2$ con $l_1\neq l_2$, possiamo scegliere due intorni disgiunti $U_1\in\mathcal{F}_{l_1}$ e $U_2\in\mathcal{F}_{l_2}$. Per la definizione di limite, definitivamente $a_n\in U_1$ e $a_n\in U_2$ cioè definitivamente $a_n\in U_1\cap U_2$, che è assurdo essendo loro disgiunti. $\blacksquare$
*Proposizione*:
Se $a_n\to l$ allora ogni sua estratta tende a $l$.
*Dimostrazione*:
Sia $\{a_{n_k}\}_n$ un estratta, allora:
$$n>\bar{n}\Rightarrow k_n\geq n\geq \bar{n}$$
dunque:
$$\forall n\geq\bar{n},\quad a_k\in U$$
$\blacksquare$

---
*Proposizione*:
Una successione $\{a_n\}_n$ converge ad $l\in\mathbb{R}$ se e solo se: $$\forall\varepsilon>0\,\exists\bar{n}:\forall n\geq\bar{n}, \quad |a_n-l|<\varepsilon$$
Una successione $\{a_n\}_n$ diverge positivamente (negativamente) se e solo se: $$\forall M\,\exists\bar{n}\geq n,\quad a_n>M\quad(<M)$$
La prima proprietà è equivalente a dire che:
$$\forall\varepsilon>0,\exists\bar{n}:\forall n\geq \bar{n}, l-\varepsilon<a_n<l+\varepsilon$$
