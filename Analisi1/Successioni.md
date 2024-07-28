---
tags: SuccessionieSerie
aliases:
- successione
---


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
*Proposizione 5.18*:
Una successione $\{a_n\}_n$ è infinitesima se e solo se la successione dei valori assoluti è infinitesima.

---
*Teorema* (Bolzano-Weierstrass):
Ogni successione limitata di numeri reali ha almeno una sottosuccessione convergente.
*Dimostrazione*:
Sia $\{a_n\}_n$ una successione limitata, allora esistono $\alpha_{0}$ e $\beta_{0}$ tali che $$
\forall m\in \mathbb{N},\,a_{m} \in I=[\alpha_{0},\beta_{0}]
$$
cioè, posto $I_{0}=[\alpha_{0},\beta_{0}]$, l'insieme:
$$
A_{0}=\left\{ m:a_{m}\in I_{0} \right\} 
$$
è infinito, ovvero $a_n$ cade infinite volte in $\alpha_{0},\beta_{0}$. Usando il metodo di bisezione costruiremo due successioni $\{a_n\}_n$ e $\{\beta_n\}_n$ tali che, posto $I_{n}=[\alpha_{n},\beta_{n}]$ e $A_{n}=\left\{ m: a_{m} \in I \right\}$, il predicato:
$$
\mathcal{P}(n):
\begin{cases}
\alpha\leq \cdots\leq\alpha_{n},\qquad \beta_{n}\leq \cdots\leq\beta_{0} \\
\beta_{n}=\alpha_{n} + \frac{\beta_{0}-\alpha_{0}}{2^{n}} \\
A_{n}\text{ è infinito}   
\end{cases}
$$
sia vero per ogni $n$, quindi in particolare $a_{n}$ appartiene infinite volte in $[\alpha_{i},\beta_{i}]$. Abbiamo già determinato $\alpha_{0}$ e $\beta_{0}$ che verificano $\mathcal{P(0)}$. Procedendo per induzione, supponiamo di aver determinato per ogni $h\leq n$ dei numeri $\alpha_{k},\beta_{k}$ in modo che sia vero $\mathcal{P}(n)$. Indichiamo con $\mu_{n}=\frac{\alpha_{n}-\beta_{n}}{2}$ il punto dell'intervallo $I_{n}$ e osserviamo che 
$$
A_{n}=\left\{ m:a_{m}\in[\alpha_{n},\mu_{n}] \right\}\cup \left\{ m:a_{m}\in[\mu_{n},\beta_{n}] \right\}.
$$
Essendo $A_{n}$ infinito, almeno uno dei due insieme deve essere infinito. Senza perdita di generalità, sia l'intervallo destro quello con infiniti elementi, allora poniamo
$$
\alpha_{n+1}=\mu_{n},\qquad \beta_{n+1}=\beta_{n}
$$
e poniamo $I_{n+1}=[\alpha_{n+1},\beta_{n+1}]$ e $A_{n+1}=\left\{ m:a_{m} \in I_{n+1} \right\}$, abbiamo che $A_{n+1}$ è infinito, che $\alpha_{n} \leq a_{n+1}$ e $\beta_{n+1}\leq\beta_{n}$, e che
$$
\beta_{n+1}-\alpha_{n+1}=\frac{\beta_{n}-\alpha_{n}}{2}=\frac{\beta_{0}-\alpha_{0}}{2^{n}}
$$
quindi $\mathcal{P}(n+1)$ è verificato.
Osserviamo che la successione $\{\alpha_n\}_n$ è debolmente crescente, mentre $\{\beta_n\}_n$ è debolmente decrescente, quindi in particolare per ogni $n$ $\alpha_{n}\leq\beta_{n}\leq \{\beta_n\}_n$, per il teorema di confronto [[Teoremi di confronto per successioni|5.22]] anche $l\in[\alpha_{0},\beta_{0}]$. Osserviamo anche che, per la [[disuguaglianza di Bernoulli]], con $a=1$ abbiamo
$$
2^{n}=(1+1)^{n}\geq (1+n)\to +\infty
$$
quindi
$$
\beta_{n}=\alpha_{n}+ \frac{\beta_{0}-\alpha_{0}}{2^n}\to l
$$
Otteniamo quindi una sottosuccessione $\{a_{k_{n}}\}_n$ tale che per ogni $n$ $$
\alpha_{n}\leq a_{k_{n}}\leq\beta_{n}
$$
quindi per il [[Teoremi di confronto per successioni#^5ede27|teorema dei carabinieri]] anche $a_{k_{n}}\to l$. $\blacksquare$

---
Le successioni possono essere anche definite per ricorrenza cioè attraverso un'espressione del tipo:
$$
a_{0}=\alpha\qquad a_{n+1}=f(a_{n})
$$
dove $f$ è una funzione che si accumula su tutti i punti di $\{a_n\}_n$.

---
*Proposizione A5.34*:
se $f:\mathbb{R}\to \mathbb{R}$ è continua e crescente, per ogni $\alpha \in \mathbb{R}$ la successione definita per ricorrenza come sopra ha limite. in particolare se $f(\alpha)=\alpha$ la successione è costante, se invece $f(\alpha)\neq \alpha$, posto
$$
\alpha_{-}=\sup\left\{ x<\alpha:f(x)=x \right\},\qquad\alpha_{+}=\inf\left\{ x>\alpha:f(x)=x \right\}
$$
si ha:
$$
\begin{gather}
f(\alpha)>\alpha \quad\Rightarrow\quad \{a_n\}_n\text{ cresce e }\lim_{ n \to \infty } a_{n}=\alpha_{+} \\
f(\alpha)<\alpha \quad\Rightarrow\quad \{a_n\}_n\text{ decresce e }\lim_{ n \to \infty } a_{n}=\alpha_{-} \\
\end{gather}
$$
*Dimostrazione*:
il caso $f(\alpha)=\alpha$ è immediato anche se va fatto per induzione. Altrimenti, da $\alpha_{-}<\alpha<\alpha_{+}$ segue
$$
\forall n,\quad \alpha_{-}<\alpha<\alpha_{+}
$$
se $\alpha_{-}=-\infty$ la disuguaglianza di sinistra è ovvia, e se $\alpha_{-}\in \mathbb{R}$ allora per la continuità di $f$ e dal teorema di permanenza del segno che $f(\alpha_{-})=\alpha_{-}$, dalla crescenza di $f$ se $a_{n}>\alpha_{-}$ allora $a_{n+1}=f(a_{n})>f(\alpha_{-})=\alpha_{-}$. L'altra disuguaglianza è analoga. Per quanto riguarda la monotonia, per il [[Teoremi e proprietà delle funzioni continue#^5c6863|Teorema degli zeri]] la funzione $f(x)-x$ ha segno costante in $(\alpha_{-},\alpha_{+})$, quindi se per esempio $f(\alpha)>\alpha$ abbiamo $f(x)>x$ per ogni $x \in (\alpha_{-},\alpha_{+})$ dunque $$
\forall n,\qquad a_{n+1}=f(a_{n})>a_{n},
$$
cioè la successione è crescente, ed ha limite $l$ con $\alpha_{-}<\alpha<\alpha_{+}$. Se fosse $l<\alpha_{+}$, in particolare sarebbe $l\in \mathbb{R}$, dunque $f$ continua in $l$ e da $a_{n}\to l$ otteniamo $a_{n+1}=f(a_{n})\to f(l)$, ma $a_{n+1}\to l$ e per l'unicità del limite $f(l)=l$, contro la definizione di $\alpha_{+}$. L'altro caso è analogo.


#SuccessionieSerie 