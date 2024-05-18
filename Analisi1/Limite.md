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

---
*Teorema*:
Siano $\{a_n\}_n$ e $\{b_n\}_n$ due successioni tali che $$a_n\to l_a,\qquad b_n\to l_b$$
Allora, se ha senso scrivere $l_a+l_b$, abbiamo $$(a_n+b_n)\to(l_a+l_b).$$
E vale lo stesso per il prodotto, se ha senso.
*Dimoostrazione*:
Iniziamo con il caso $l_a,l_b\in\mathbb{R}$: fissato $\varepsilon>0$, abbiamo definitivamente $$|a_n-l_a|<\varepsilon,\quad|b_n-l_b|<\varepsilon$$
Per disuguaglianza triangolare otteniamo: $$|(a_n+b_n)-(l_a+l_b)|=|(a_n-l_a)+(b_n-l_b)|\leq |a_n-l_a|+|b_n-l_b|$$
Quindi definitivamente: $$|(a_n+b_n)-(l_a+l_b)|<2\varepsilon$$
Supponiamo adesso il caso $l_a=+\infty$ quindi $l_b$ può essere o no $+\infty$ ma in ogni caso è inferiormente limitato. In particolare $b_n$ converge o diverge positivamente. Vale a dire: $$\exists K\in\mathbb{R}:\forall n\in\mathbb{N},\quad b_n\geq K$$ (è limitata inferiormente), quindi $$a_n+b_n\geq a_n+K$$
poiché $a_n\to+\infty$, per ogni $M\in\mathbb{R}$ definitivamente $a_n>M$, quindi $$a_n+b_n>M+K$$ dunque $$(a_n+b_n)\to+\infty$$Passiamo a dimostrare il caso del prodotto dato che gli altri casi della somma sono analoghi. Iniziamo col caso reale. osserviamo che:$$|a_nb_n-l_al_b|=|a_nb_n-l_ab_n+l_ab_n-l_al_b|\leq|a_n-l_a|\cdot|b_n|+|l_a|\cdot|b_n-l_b|$$
Dato che $\{b_n\}_n$ converge, è limitata, pertanto esiste $K>0$ tale che per ogni $n$ si ha che $|b_n|\leq K$, scelto $\varepsilon>0$, per ipotesi definitivamente vale: $$|a_nb_n-l_al_b|\leq |a_n-l_a|\cdot|b_n|+|l_a|\cdot|b_n-l_b|\leq K\varepsilon+|l_a|\varepsilon\leq (K+|l_a|)\varepsilon$$
Non ci rimane che il caso $l_a=+\infty$ e $l_b>0$