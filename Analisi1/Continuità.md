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
#continuità