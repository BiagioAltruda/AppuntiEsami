una funzione $f:a\to\mathbb{R}$ che per un certo $x_{*}\in A$ verifica $$
\forall \left\{ x_{n} \right\}_{n} \subset A,\qquad x_{ n}\to x_{*}\Rightarrow f(x_{n})\to f(x_{*})  
$$ si dice continua in $x_{*}$, una funzione continua in ogni punto del suo dominio si dice continua.

---
*Teorema 5.34*: 
Se $f$ e $g$ sono continue in $x_{*}$ allora lo sono anche $f+g$, $fg$ e $\frac{f}{g}$ se $g(x_{*})\neq 0$.
*Dimostrazione*:
Sia $x_{n}\to x_{*}$; allora $f(x_{n})\to f(x_{*})$, e lo stesso per $g$. Da questo segue che: $$
(f+g)(x_{n})=f(x_{n})+g(x_{n})\to f(x_{*})+g(x_{*})=(f+g)(x_{*})
$$
Le altre si fanno allo stesso modo. $\blacksquare$

---
*Proposizione 6.3*:
Se $f$ è una funzione reale e $x_{*}\in \mathbb{R}$ è un punto di accumulazione di dom$f$ allora $f$ è continua in $x_{*}$ se e solo se $\lim_{ x \to x_{*} }f(x)=f(x_{*})$.
*Dimostrazione*:
Usando da definizione di continuità in $x_{*}$: $$
\forall \left\{ x_{n} \right\}_{n} \subset \text{dom}f,\qquad x_{n}\to x_{*}\Rightarrow f(x_{n})\to f(x_{*})\qquad\qquad 1)
$$ invece per il [[Limite#^604ab5| Teorema 6.2]], $f(x)\to f(x_{*})$ equivale a:
$$
\forall \left\{ x_{n} \right\}_{n} \subset \text{dom}f\setminus \left\{ x_{*} \right\},\qquad x_{n}\to x_{*}\Rightarrow f(x_{n})\to f(x_{*})\qquad\qquad 2)
$$
è chiaro che la prima formula implica la seconda, dobbiamo solo dimostrare il viceversa, sia allora $\{x_{n}\}_n$ di punti di dom$f$, convergente a $x_{*}$, e proviamo che $f(x_{n})\to f(x_{*})$. Se definitivamente $x_{n}=x_{*}$ questo è ovvio; se definitivamente$x_{n}\neq x_{*}$ questo discende da 2), nel caso che rimane, dividiamo $\{x_{n}\}_n$ in due sottosuccessioni: quella dei termini per i quali $x_{n}=x_{*}$ (chiamiamola $\{x_{1_{n}}\}_n$)e quella dei termini per i quali $x_{n}\neq x_{*}$ (chiamiamola $\{x_{2_{n}}\}_n$). Entrambe convergono a $x_{*}$, ma la prima è costantemente uguale a $x_{*}$, mentre la seconda è sempre diversa da $x_{*}$, dunque per le considerazioni precedenti: $$
f(x_{1_{n}})\to f(x_{*})\qquad\qquad f(x_{2_{n}})\to f(x_{*}) 
$$
e da questo segue che $f(x_{n})\to f(x_{*})$ applicando la proposione 5.15 $\blacksquare$ ????

---
*Proposizione 6.4*:
Se $f$ è una funzione reale che ha limite $l\in \mathbb{R}$ quando $x$ tende ad un punto di accumulazione $x_{*}$ del suo dominio, la funzione:$$
\tilde{f}(x)=\Big\{ f(x)\quad \text{se }x \neq x_{*}, \quad l\quad \text{se } x=x_{*} 
$$ è continua in $x_{*}$.
La funzione $\tilde{f}$ si dice *estensione continua* di $f$ in $x_{*}$.

---

*Teorema 6.5*:
se $f,g,h$ sono tre funzioni reali aventi lo stesso dominio e $x_{*}$ è un punto di accumulazione del loro dominio, allora:
1. se in dom$f$ si ha $f(x)\leq g(x)$, e se $f(x)\to l_{f}$ e $g(x)\to l_{g}$ per $x\to x_{*}$ allora $l_{f}\leq l_{g}$.
2. se in dom$f$ si ha$f(x)\leq g(x)$, e se $f\to +\infty$ (o $g\to-\infty$) per $x\to x_{*}$ allora anche $g(x)\to +\infty$ (o $f\to-\infty$).
3. se in dom$f$ si ha  $f(x)\leq g(x)\leq h(x)$, e se $\lim_{ x \to x_{*} }f(x)=\lim_{ x \to x_{*} }h(x)=l$ allora esiste anche $\lim_{ x \to x_{*} }g(x)$ ed è uguale a $0$.

---
*Teorema 6.6*:
siano $f,g$ due funzioni reali aventi lo stesso dominio e tali che $f(x)\to l_{f}$ e $g(x)\to l_{g}$ per $x\to x_{*}$, dove $x_{*}$ è un punto di accumulazione del loro dominio, si ha che:
$$
\begin{gather}
1)\quad \lim_{ x \to x_{*} } (f(x)+g(x))=l_{f}+l_{g},\\
2)\quad \lim_{ x \to x_{*} }(f(x)\cdot g(x))=l_{f}\cdot l_{g},\\
3)\quad \lim_{ x \to x_{*} } \frac{f(x)}{g(x)}=\frac{l_{f}}{l_{g}},
\end{gather} 
$$
a meno di forme di indeterminazione.

---
*Teorema 6.11*:
Siano $f,g$ funzioni reali e sia $$
\lim_{ x \to x_{*} } f(x)=y_{*},\quad \lim_{ x \to y_{*} } g(x)=l
$$
dove $x_{*}$ è un punto di accumulazione del dominio di $f\circ g$ e $y_{*}$ punto di accumulazione del dominio di $g$. Se vale almeno una delle seguenti ipotesi:
1. $\exists W_{0}\in\mathcal{F_{x_{*}}}\text{ tale che }f(x)\neq y_{*}, \forall x\in \text{dom}(f\circ g)\cap W_{0}\setminus \left\{ x_{*} \right\}$,
2. $y_{*}\in \text{dom}g\text{ e }g(y_{*})=l$,
allora $\lim_{ x \to x_{*} }g(f(x))=l$.
*Dimostrazione*:
Fissiamo $U\in \mathcal{F_{l}}$: l'ipotesi su $g$ dà $$
\exists V\in \mathcal{F_{y_{*}}}:\forall y\in \text{dom}g\cap V\setminus \left\{ y_{*} \right\},\quad g(y)\in U.
$$
Dato che $V$ è un intorno di $y_{*}$, l'ipotesi su $f$ dà
$$
\exists W_{1}\in \mathcal{x_{*}}:\forall x \in \text{dom}f\cap W_{1}\setminus \left\{ x_{*} \right\} ,\quad f(x)\in V.
$$
Per brevità poniamo:
$$
A=\text{dom}(f\circ g)\subset \text{dom}f,\qquad B=f(A)\subset \text{dom}g.
$$
Dalle formule precedenti, osservando che $x \in A\Rightarrow f(x)\in B$, ricaviamo
$$
\begin{gather}
x \in A\cap W_{1}\setminus \left\{ x_{*} \right\}\quad\Rightarrow \quad f(x)\in B\cap V\\
y\in B\cap V\setminus \left\{ y_{*} \right\} \quad\Rightarrow\quad g(y)\in U
\end{gather}
$$
Se in entrambe le formule ci fosse scritto $B\cap V$, oppure $B\cap V\setminus \left\{ y_{*} \right\}$, potremmo sostituire $y$ con $f(x)$ e ottenere la tesi $g(f(x))\in U$. Se vale l'ipotesi 1. poniamo $W=W_{0}\cap W_{1}$: dalla prima formula di sopra otteniamo
$$
x \in A\cap W\setminus \left\{ x_{*} \right\} \quad\Rightarrow\quad f(x)\in B\cap V\setminus \left\{ y_{*} \right\},
$$
che insieme alla seconda dà
$$
x \in A \cap W\setminus \left\{ x_{*} \right\} \quad\Rightarrow\quad g(f(x))\in U,
$$
che è la tesi. Se invece vale l'ipotesi 2., la seconda formula diviene
$$
y\in B\cap V \quad\Rightarrow\quad g(y)\in U
$$
che unita alla prima dà ancora il risultato di prima, ponendo $W=W_{1}$.$\blacksquare$

---
Una definizione alternativa di continuità è che se $f:A\to \mathbb{R} \text{ e } x_{*}\in A$, si dice che $f$ è continui in $x_{*}$ se:
$$
\forall U \in \mathcal{F_{f(x_{*})}},\exists V \in \mathcal{F_{f(x_{*})}}:\forall x \in A \cap V, \quad f(x)\in U
$$
Vale anche la seguente
*Proposizione 6.17*: Sia $f:A\to \mathbb{R}$, allora la definizione data sopra è equivalente a:
$$
\begin{align}

\forall U\in \mathcal{F_{f(x_{*})}}, \exists V\in \mathcal{F_{x_{*}}}: f(A\cap V)\subset U\qquad 1) \\

\forall U \in \mathcal{F_{f(x_{*})}}, f^{-1}(U)\text{ contiene l'intersezione con } A\text{ di un intorno di }x_{*}\quad 2)\\

x_{*}\text{è punto isolato di }A \text{ oppure }\lim_{ x \to x_{*} } f(x)=f(x_{*})\qquad 3)\\
\forall \varepsilon>0,\exists\delta>0:\forall x \in A,\quad|x-x_{*}|<\delta \quad\Rightarrow\quad |f(x)-f(x_{*})|<\varepsilon\quad 4)
\end{align}
$$
*Dimostrazione*:
$1)$ e $2)$ sono riscritture della definizione di sopra. Dimostriamo che $1)\Rightarrow 3)$, se $f$ è continua in $x_{*}$, questo può essere punto isolato di $A$ (allora ho finito), oppure può essere punto di accumulazione di $A$; in questo caso, essendo $A\cap V\setminus \left\{ x_{*} \right\}$ la continuità di $f$ implica che
$$
\forall U \in \mathcal{F_{f(x_{*})}},\exists V \in \mathcal{F_{f(x_{*})}}:\forall x \in A \cap V, \quad f(x)\in U
$$
che è precisamente $\lim_{ x \to x_{*} }f(x)=f(x_{*}).$ Proviamo il viceversa, se $x_{*}$ è isolato, per definizione esiste un intorno $V_{0}\in \mathcal{F_{x_{*}}}$ tale che $A\cap V_{0}=\left\{ x_{*} \right\}$; allora, scelto un qualsiasi intorno $U$ di $f(x_{*})$ certamente $x \in A\cap V_{0}\Rightarrow x=x_{*}\Rightarrow f(x)=f(x_{*})\in U$ ([[Limite|Proposizione 5.1]]). Se invece $x_{*}$ è di accumulazione e $\lim_{ x \to x_{*} }f(x)=f(x_{*})$, per definizione di limite, fissato $U\in \mathcal{F_{f(x_{*})}}$ esiste $V\in \mathcal{F_{x_{*}}}$ tale che $$
\forall x \in A\cap V\setminus \left\{ x_{*} \right\} ,\qquad f(x)\in U
$$
ma anche $f(x_{*})\in U$, quindi per ogni $x \in A\cap V$ è $f(x)\in U$.
Infine $4)$ è equivalente a $1)$ perché $x_{*}$ e $f(x_{*})$ sono numeri reali: ogni intorno di un numero reale $a$ contiene un intervallo della forma $\left\{ x:|x-a|<\varepsilon \right\}$, e viceversa ogni intervallo di questo tipo è un intorno di $a$. $\blacksquare$


Seguono i primi [[Teoremi e proprietà delle funzioni continue]].
#continuità