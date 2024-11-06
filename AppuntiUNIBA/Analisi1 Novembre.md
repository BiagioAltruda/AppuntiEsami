*Definizione*:
Sia $A\subset \mathbb{R}$. Si dice successione numerica di elementi di $A$ ogni funzione $$
f:\mathbb{N}\to A.
$$
Tale successione si denota col simbolo $(a_{n})_{n\in \mathbb{N}}$, dove $\forall n\in \mathbb{N},\,f(n)=a_{n}\in A$.

*Definizione*:
Sia $(a_{n})_{n\in \mathbb{N}}$ una successione di numeri reali. Si dice che $(a_{n})_{n\in \mathbb{N}}$ è monotona crescente  se: $$
\forall n,m\in \mathbb{N},\,n<m:\, a_{n}\leq a_{m}.
$$
Si dice, invece, che $(a_{n})_{n\in \mathbb{N}}$ è monotona decrescente se: $$
\forall n,m\in \mathbb{N},\, n<m:\, a_{m}\leq a_{n}.
$$
Inoltre si dice che $(a_{n})_{n\in \mathbb{N}}$ è strettamente monotona crescente (rispettivamente strettamente monotona decrescente) se: $$
\forall n,m\in \mathbb{N},\,n<m:\, a_{n}<a_{m}\qquad(a_{m}<a_{n} \text{ rispettivamente}).
$$
*Proposizione*:
Sia $(a_{n})_{n\in \mathbb{N}}$ una successione di numeri reali. I seguenti fatti sono equivalenti:
1. $(a_{n})_{n\in \mathbb{N}}$ è monotona crescente (decrescente).
2. $\forall n\in \mathbb{N}:\, a_{n}\leq a_{n+1}\,(a_{n+1}\leq a_{n})$.

*Dimostrazione*:
$1)\implies 2)$. Segue direttamente dalla definizione di monotonia. Dato che $\forall n\in \mathbb{N},\,m=n+1\implies n<m\implies a_{n}\leq a_{n+1}$.
$2)\implies 1)$. Supponiamo che $\forall n\in \mathbb{N},\,a_{n}\leq a_{n+1}$. Proviamo che $\forall n,m\in \mathbb{N}\,n<m:\, a_{n}\leq a_{m}$.
Fissiamo $n,m\in \mathbb{N}$, con $n<m$. Poniamo $k=m-n\in \mathbb{N},\,k\geq 1$. Vogliamo provare che $a_{n}\leq a_{n+k}$. Se $k=1$, allora $a_{n}\leq a_{n+1}$ per ipotesi. Procediamo per induzione su $k$. Abbiamo già verificato $k=1$. Supponiamo che $a_{n}\leq a_{n+k}$ e dimostriamo per $k+1$. Allora: $$
a_{n}\leq a_{n+k}\leq a_{(n+k)+1}=a_{n+(k+1)}.
$$
Da cui $a_{n}\leq a_{n+(k+1)}$. Segue che $\forall k\in \mathbb{N},\,k\geq1,\,a_{n}\leq a_{n+k}$, concludiamo che $a_{n}\leq a_{m}\,\blacksquare$.

*Proposizione*:
Sia $(a_{n})_{n\in \mathbb{N}}$ una successione di numeri reali. I seguenti fatti sono equivalenti:
1. $(a_{n})_{n\in \mathbb{N}}$ è strettamente monotona crescente (decrescente).
2. $\forall n\in \mathbb{N}:\, a_{n}< a_{n+1}\,(a_{n+1}<a_{n})$.

*Dimostrazione*:
Analoga alla precedente.

*Esempi*:
$(1)_{n\in \mathbb{N}}$, $f:\mathbb{N}\to \mathbb{R}:\, \forall n\in \mathbb{N},\, f(n)=1$. Il grafico di $f$: $G_{f}=\left\{ (n,f(n))|\, n\in \mathbb{N} \right\}=\left\{ (n,1)|\,n\in \mathbb{N} \right\}.$
$\forall n\in \mathbb{N},\, a_{n}=a_{n+1}\implies a_{n}\leq a_{n+1}$ e anche $a_{n+1}\leq a_{n}$. Quindi $(1)_{n\in \mathbb{N}}$ è sia monotona crescente che monotona decrescente, ma non strettamente.

$\left( \frac{1}{n+1} \right)_{n\in \mathbb{N}}$, $f:\mathbb{N}\in \mathbb{R}:\, \forall n\in \mathbb{N}, f(n)= \frac{1}{n+1}$. Questa è una successione strettamente monotona decrescente, ossia: $$
\forall n,m\in \mathbb{N},\,n<m: a_{m}<a_{n} \iff \forall n,m\in \mathbb{N},n<m: \frac{1}{m+1}< \frac{1}{n+1} \iff \forall n\in \mathbb{N},\, \frac{1}{n+1}< \frac{1}{n}.
$$
*Definizione*:
Sia $(a_{n})_{n\in \mathbb{N}}$ successione di numeri reali. Sia $l\in \overline{\mathbb{R}}$. Si dice che la successione $(a_{n})_{n\in \mathbb{N}}$ tende a $l$ per $n$ tendente a $+\infty$ se: $$
\forall V\in \mathcal{J}_{l},\, \exists \nu\in \mathbb{N}: \forall n\in \mathbb{N},\, n\geq \nu \implies a_{n}\in V.
$$
In tal caso si scrive: $$
\lim_{ n \to +\infty } a_{n}=l.
$$
*Definizione*:
Sia $P(n)$ una proprietà indicizzata da $n\in \mathbb{N}$. Si dice che $P(n)$ è vera definitivamente se: $\exists \nu \in \mathbb{N}$ tale che $\forall n\in\mathbb{N},\,n\geq \nu$, $P(n)$ è vera.

*Osservazione*:
Diremo che $(a_{n})_{n}$ tende a $l$, per $n$ che tende a $+\infty$, si esprime dicendo: $$
\forall V\in \mathcal{J}_{l}:\,a_{n}\in V \text{ definitivamente}.
$$
*Definizione*:
Sia $P(n)$ una proprietà indicizzata da $n\in \mathbb{N}$. Si dice che $P(n)$ è vera frequentemente se: $P(n)$ è vera per infiniti indici. Ovvero: $$
\forall k\in \mathbb{N},\,\exists n\in \mathbb{N},\,n\geq k \text{ tale che }P(n) \text{ è vera}.
$$
*Osservazione*:
$P(n)$ è vera definitivamente allora $P(n)$ è vera frequentemente.

*Dimostrazione*:
$P(n)$ vera definitivamente vuol dire che $\exists \nu \in \mathbb{N}:\, \forall n\in \mathbb{N},\,n\geq \nu$: $P(n)$ è vera. Vogliamo provare che $\forall k\in \mathbb{N},\,\exists n\in \mathbb{N},\,n\geq k$ tale che $P(n)$ è vera.
Sia $k\in \mathbb{N}$, esiste $n\in \mathbb{N}$, tale che $n\geq \max\left\{ k,\nu \right\}$ tale che $P(n)$ è vera $\blacksquare$.

*Teorema*(unicità del limite di successioni):
Sia $(a_{n})_{n\in \mathbb{N}}$ successione di numeri reali. Se $(a_{n})_{n\in \mathbb{N}}$ ammette un limite per $n$ che tende a $+\infty$, allora questo limite è unico.

*Dimostrazione*:
Per assurdo, se $(a_{n})_{n\in \mathbb{N}}$ ammettesse due limiti distinti, $l_{1},l_{2}\in\overline{\mathbb{R}}$ tali che $\lim_{ n \to +\infty }a_{n}=l_{1}$ e $l_{2}$. Poiché $l_{1}\neq l_{2}$, per il principio di separazione degli intorni, $\exists V_{1}\in \mathcal{J}_{l_{1}},\,\exists V_{2}\in \mathcal{J}_{l_{2}}$ tali che $V_{1}\cap V_{2}=\emptyset$. Poiché $(a_{n})_{n\in \mathbb{N}}$ tende ad $l_{1}$, in corrispondenza di $V_{1},\,\exists \nu_{1}\in \mathbb{N}$ tale che $\forall n\in \mathbb{N},\,n\geq \nu_{1}$ (definitivamente) si ha che $a_{n}\in V_{1}$. Vale l'analogo per $l_{2}$, quindi in corrispondenza di $V_{2},\exists \nu_{2}\in \mathbb{N}$ tale che $\forall n\in \mathbb{N},\, n\geq \nu_{2}$ (definitivamente) si ha che $a_{n}\in V_{2}$. Segue che posto $\nu_{3}=\max\left\{ \nu_{1},\nu_{2} \right\}$, si ha $\forall n\in \mathbb{N},\, n\geq \nu_{3}:a_{n}\in V_{1}\cap V_{2}\neq \emptyset$, che produce una contraddizione in quanto avevamo supposto che $V_{1}\cap V_{2}=\emptyset\,\blacksquare$.

*Esempio*:
La successione $((-1)^{n})_{n\in \mathbb{N}}$, $f:\mathbb{N}\to \mathbb{R}:\,\forall n\in \mathbb{N},\, f(n)=(-1)^{n}$. Ovvero $a_{n}=(-1)^{n},\, \forall n\in \mathbb{N}$.
Questa successione non ammette limite, perché esistono intorni di $1$ o $1$ per i quali $a_{n}$ non gli appartiene, definitivamente.

*Definizione*:
Sia $(a_{n})_{n\in \mathbb{N}}$ una successione di numeri reali. Sia $l\in\overline{\mathbb{R}}$. supponiamo che $\exists \lim_{ n \to +\infty }a_{n}=l\in\overline{\mathbb{R}}$, allora: $$
\begin{cases}
l\in\overline{\mathbb{R}} &\text{ si dice che } a_{n} \text{ converge ad }l \\
l=+\infty&\text{ si dice che }a_{n} \text{ diverge positivamente, e si scrive: } \lim\limits_{ n \to +\infty } a_{n}=+\infty \\
l=-\infty&\text{ si dice che } a_{n} \text{ diverge negativamente, e si scrive } \lim\limits_{ n \to +\infty } a_{n}=-\infty.
\end{cases}
$$

$1):\,l\in \mathbb{R},\, \lim\limits_{ n \to +\infty }a_{n}=l$ vuol dire che $$
\forall\varepsilon>0,\,\exists \nu \in \mathbb{N}\text{ tale che }\forall n\in \mathbb{N},\,n\geq \nu:\, |a_{n}-l|<\varepsilon,
$$
ovvero: $$
\forall\varepsilon>0,\, \exists \nu \in \mathbb{N} \text{ tale che }\forall n\in \mathbb{N},\,n\geq \nu:\, a_{n}\in]l-\varepsilon,l+\varepsilon[.
$$
$2):l=+\infty\,(-\infty),\,\lim\limits_{ n \to +\infty }a_{n}=+\infty\,(-\infty)$ vuol dire che $$
\forall k\in \mathbb{R},\,k>0\,\exists \nu \in \mathbb{N}\text{ tale che }\forall n\in \mathbb{N},\,n\geq \nu:\, a_{n}>k \,(a_{n}<-k)
$$
ovvero: $$
\forall V=]k,+\infty[\,\,(V=]-\infty,-k[)\,\, \exists \nu \in \mathbb{N} \text{ tale che }\forall n\in \mathbb{N},\,n\geq \nu: a_{n}\in]k,+\infty[\,\,(a_{n}\in]-\infty,-k[).
$$
*Definizione*:
Sia $(a_{n})_{n\in \mathbb{N}}$ una successione di numeri reali. Si dice che $(a_{n})_{n\in \mathbb{N}}$ è limitata superiormente (inferiormente) se: $$
\exists M>0 \text{ tale che } a_{n}\leq M(a_{n}\geq -M)\, \forall n\in \mathbb{N}.
$$
Si dice che $(a_{n})_{n\in \mathbb{N}}$ è limitata se è limitata sia superiormente che inferiormente. Ossia che: $$
\exists M>0 \text{ tale che }\forall n\in \mathbb{N},\, |a_{n}|\leq M.
$$
*Esempi*:
$((-1)^{n})_{n\in \mathbb{N}}$ è limitata da $M=1$.
$(2)_{n\in \mathbb{N}}$ è limitata da, per esempio $M=3$.
$b_{n}=\left( \frac{1}{n+1} \right)_{n\in \mathbb{N}}$, allora $b_{n}\leq 1$ e anche $b_{n}>0$. Allora: $|b_{n}|= \frac{1}{n+1}\leq 1$.
Mentre $(n)_{n\in \mathbb{N}}$ non è limitata superiormente.

*Proposizione*:
Sia $(a_{n})_{n\in\mathbb{N}}$ una successione di numeri reali convergente. Allora $(a_{n})_{n\in\mathbb{N}}$ è limitata.

*Dimostrazione*:
Sia $l\in \mathbb{R}$ tale che $\lim\limits_{ n \to +\infty }a_{n}=l$. Pertanto $\forall\varepsilon>0 \,\exists \nu \in \mathbb{N}$ tale che $\forall n\in \mathbb{N},\,n\geq \nu:\, |a_{n}-l|<\varepsilon.$ Cioè $l-\varepsilon<a_{n}<l+\varepsilon$. Scelto $\varepsilon=1,\,\exists \nu \in \mathbb{N},$ tale che $\forall n>\nu,\, l-1<a_{n}<l+1$. Consideriamo $M=\max\left\{ a_{0},a_{1},\dots,a_{\nu-1},l+1 \right\}$, e sia $N=\min\left\{ a_{0},a_{1},\dots,a_{\nu-1},l-1 \right\}$. Segue che $\forall n\in \mathbb{N}, N\leq a_{n}\leq M$. Quindi $(a_{n})_{n\in\mathbb{N}}$ è limitata.

*Definizione*:
Sia $(a_{n})_{n\in\mathbb{N}}$ una successione di numeri reali. Si chiama estremo superiore della successione $(a_{n})_{n\in\mathbb{N}}$, e si denota con $\sup\limits_{n\in\mathbb{N}} (a_{n})$, l'estremo superiore dell'insieme: $\left\{ a_{n}|\,n\in \mathbb{N} \right\}$. 
Mentre si chiama estremo inferiore della successione $(a_{n})_{n\in\mathbb{N}}$, e si denota con $\inf\limits_{n\in \mathbb{N}}(a_{n})$, l'estremo inferiore dell'insieme: $\left\{ a_{n}|\,n\in \mathbb{N} \right\}$.

*Definizione*:
Una successione $(a_{n})_{n\in\mathbb{N}}$ si dice infinitesima se $\exists \lim\limits_{ n \to +\infty }a_{n}=0$.

*Osservazione*:
Se $\lim\limits_{ n \to \infty }a_{n}=l\in \mathbb{R}\iff \exists \lim\limits_{ n \to \infty }a_{n}-l=0$, ossia la successione $(a_{n}-l)_{n\in \mathbb{N}}$ è infinitesima.

*Teorema*:
Siano $(a_{n})_{n\in\mathbb{N}}$ e $(b_{n})_{n\in\mathbb{N}}$ successioni di numeri reali. Supponiamo che $\exists \lim\limits_{ n \to \infty }a_{n}=a\in\overline{\mathbb{R}}$ e $\exists \lim\limits_{ n \to \infty }b_{n}=b\in\overline{\mathbb{R}}$. Allora la successione: $(a_{n}+b_{n})_{n\in \mathbb{N}}$ ammette limite $a+b$ purché tale $a+b$ non produca una forma indeterminata in $\overline{\mathbb{R}}$. Risulta in tal caso che $$
\lim\limits_{ n \to \infty } (a_{n}+b_{n})=\lim\limits_{ n \to \infty } a_{n}+\lim\limits_{ n \to \infty } b_{n}.
$$
*Dimostrazione*:
Supponiamo che $a,b\in \mathbb{R}$. Verifichiamo che $\lim\limits_{ n \to \infty }(a_{n}+b_{n})=a+b\in \mathbb{R}$.
Pertanto vogliamo provare che $$
\forall\varepsilon>0,\, \exists \nu \in \mathbb{N}:\,\forall n\in \mathbb{N},\,n\geq \nu: |a_{n}+b_{n}-(a+b)|<\varepsilon.
$$
Ovvero: $$
a+b-\varepsilon<a_{n}+b_{n}<a+b+\varepsilon.
$$
Sia $\varepsilon>0$. Poiché $\exists \lim\limits_{ n \to \infty }a_{n}=a$ e $\exists \lim\limits_{ n \to \infty }b_{n}=b$, in corrispondenza di $\frac{\varepsilon}{2}>0$: $$
\exists \nu_{1}\in \mathbb{N} \text{ tale che } \forall n\in \mathbb{N},\,n\geq \nu_{1}: a-\frac{\varepsilon}{2}<a_{n}<a+\frac{\varepsilon}{2}
$$
E anche $$
\exists \nu_{2}\in \mathbb{N} \text{ tale che }\forall n\in \mathbb{N},\,n\geq \nu_{2}: b-\frac{\varepsilon}{2}<b_{n}<b+\frac{\varepsilon}{2}.
$$
Posto $\nu_{3}=\max\left\{ \nu_{1},\nu_{2} \right\}$, si ha che $$
\forall n\in \mathbb{N},\,n\geq \nu_{3}:\, a-\frac{\varepsilon}{2}<a_{n}<a-\frac{\varepsilon}{2},\, b-\frac{\varepsilon}{2}<b_{n}<b+\frac{\varepsilon}{2} \implies
$$
E sommando membro a membro:
$$
a+b-\varepsilon<a_{n}+b_{n}<a+b+\varepsilon
$$
Allora $\exists \lim\limits_{ n \to \infty }(a_{n}+b_{n})=a+b\,\blacksquare$.

*Osservazione*:
Se $a=+\infty,\,b=-\infty$ oppure $a=-\infty,\,b=+\infty$, non possiamo dedurre alcuna informazione sul comportamento della successione $(a_{n}+b_{n})_{n\in \mathbb{N}}$.

*Proposizione*:
Sia $(a_{n})_{n\in\mathbb{N}}$ una successione di numeri reali. Sia $l\in \mathbb{R}$, supponiamo che $\exists \lim\limits_{ n \to \infty }a_{n}=l$. Allora $\exists \lim\limits_{ n \to \infty }|a_{n}|=|l|$.

*Dimostrazione*:
Vogliamo provare che $\forall \varepsilon>0,\,\exists \nu \in \mathbb{N},\,$ tale che $\forall n\in \mathbb{N},\,n\geq \nu: ||a_{n}|-|l||<\varepsilon$.
Sia $\varepsilon>0$. Per ipotesi $\exists \lim\limits_{ n \to \infty }a_{n}=l\in \mathbb{R}$, in corrispondenza di $\varepsilon>0$: $$
\exists \nu \in \mathbb{N} \text{ tale che }\forall n\in \mathbb{N},\,n\geq \nu:\, |a_{n}-l|<\varepsilon.
$$
Segue che $\forall n\in \mathbb{N},\,n\geq \nu$:
$$
||a_{n}|-|l||\leq|a_{n}-l|<\varepsilon,
$$
$$
\forall n\in \mathbb{N},\,n\geq \nu: ||a_{n}|-|l||<\varepsilon\blacksquare.
$$

*Osservazione*:
Il viceversa della proposizione è falso, ad esempio sia $(a_{n})_{n\in\mathbb{N}}=((-1)^{n})_{n\in \mathbb{N}}$.
Allora la successione $((-1)^{n})_{n\in \mathbb{N}}$ non ammette limite, ma $(|(-1)^{n}|)_{n\in \mathbb{N}}=(1)_{n\in \mathbb{N}}$ converge ad 1.

*Proposizione*:
Sia $(a_{n})_{n\in\mathbb{N}}$ una successione di numeri reali. Allora risulta vera la seguente equivalenza:
1. $\exists \lim\limits_{ n \to \infty }a_{n}=0$
2. $\exists \lim\limits_{ n \to \infty }|a_{n}|=0$.

*Dimostrazione*:
Basta verificare che $2)\implies1)$. Supponiamo che $\exists \lim\limits_{ n \to \infty }|a_{n}|=0$ e proviamo che $$
\forall\varepsilon>0\,\exists \nu \in \mathbb{N} \text{ tale che }\forall n\in \mathbb{N},\,n\geq \nu: |a_{n}|<\varepsilon.
$$
Sia quindi $\varepsilon>0$. Poiché $\exists \lim\limits_{ n \to \infty }|a_{n}|=0$, in corrispondenza di $\varepsilon>0$: $$
\exists \nu \in \mathbb{N} \text{ tale che } \forall n\in \mathbb{N},\,n\geq \nu: |a_{n}|=||a_{n}||<\varepsilon\,\blacksquare.
$$

*Esempio*:
Sia $(a_{n})_{n\in\mathbb{N}}=\left( \frac{(-1)^{n}}{n} \right)_{n\in \mathbb{N} \wedge n\geq 1}$. Poiché $\exists \lim\limits_{ n \to \infty } \frac{1}{n}=0$, allora la successione $(a_{n})_{n\in\mathbb{N}}$ è infinitesima, dato che $\frac{|(-1)^{n}|}{n}=\frac{1}{n},\,\forall n\in \mathbb{N},\,n\geq 1$. Riconosciamo che $\lim\limits_{ n \to \infty } \frac{1}{n}=0$, ossia $$
\forall\varepsilon>0,\, \exists \nu \in \mathbb{N} \text{ tale che } \forall n\in \mathbb{N},\,n\geq n: \frac{1}{n}<\varepsilon.
$$
Sia $\varepsilon>0$. Per la proprietà archimedea applicata a $\varepsilon^{-1}$: $\exists \nu \in \mathbb{N}$ tale che $\nu>\varepsilon^{-1}=\frac{1}{\varepsilon}$. Allora $\forall n\in \mathbb{N},\,n\geq \nu: n> \frac{1}{\varepsilon}\iff \frac{1}{n}<\varepsilon$.
Concludiamo che $\lim\limits_{ n \to \infty } \frac{1}{n}=0$.

*Teorema*(permanenza del segno per successioni):
Sia $(a_{n})_{n\in\mathbb{N}}$ una successione di numeri reali. Supponiamo che $\exists \lim\limits_{ n\to \infty}a_{n}=l\in \mathbb{R}$. Allora valgono le seguenti implicazioni: 
1. $l>0 \implies a_{n}>0$ definitivamente
2. $l<0 \implies a_{n}<0$ definitivamente.

*Dimostrazione*:
1. Supponiamo che $l>0,\,l\in \mathbb{R}$, verifichiamo che $a_{n}>0$ definitivamente. Ovvero che $$
\exists \nu \in \mathbb{N}\text{ tale che } \forall n\in \mathbb{N},\,n\geq \nu: a_{n}>0.
$$
	Per ipotesi si ha che $\exists \lim\limits_{ n \to \infty }a_{n}=l>0$. Pertanto $$
\forall\varepsilon>0 \exists \nu \in \mathbb{N}\text{ tale che }\forall n\in \mathbb{N},\,n\geq \nu: |a_{n}-l|<\varepsilon.
$$
	Sia $\varepsilon>0$ tale che $l-\varepsilon>0$. In corrispondenza di questo $\varepsilon$: $$
\exists \nu \in \mathbb{N}\text{ tale che }\forall n\in \mathbb{N},\,n\geq \nu: 0< l-\varepsilon<a_{n}<l+\varepsilon.
$$
	Segue che $a_{n}>0$ definitivamente.
2. Supponiamo che $\exists \lim\limits_{ n \to \infty }a_{n}=l=+\infty$. Ossia $$
\forall k>0 \exists \nu \in \mathbb{N}\text{ tale che }\forall n\in \mathbb{N},\,n\geq \nu: a_{n}>k.
$$
	Sia, ad esempio, $k=1$. In corrispondenza di tale $k$, $\exists \nu \in \mathbb{N}$ tale che $\forall n\in \mathbb{N},\,n\geq \nu$ tale che $a_{n}>1>0\,\blacksquare$.
Il caso $l<0$ si dimostra allo stesso modo.

*Controesempio*:
$l=0$. $\left( \frac{(-1)^{n}}{n} \right)_{n\in \mathbb{N}}$ tende a $l=0$ ma i termini di $(a_{n})_{n\in\mathbb{N}}$ cambiano segno.

*Corollario*:
Sia $(a_{n})_{n\in\mathbb{N}}$ una successione di numeri reali. Supponiamo che $\exists \lim\limits_{ n \to \infty }a_{n}=l\in\overline{\mathbb{R}}$. Allora valgono le seguenti implicazioni:
1. $a_{n}\geq0$ definitivamente, allora $l\geq 0$
2. $a_{n}\leq 0$ definitivamente, allora $l\leq 0$.

*Dimostrazione*:
Dimostriamo $1)$. Supponiamo che $a_{n}\geq 0$ definitivamente. Se per assurdo $l<0$, allora dal teorema della permanenza del segno segue che $a_{n}<0$ definitivamente, che è assurdo, in quanto, definitivamente $0\leq a_{n}<0 \implies 0<0$ $\blacksquare$.

*Proposizione*(criterio del confronto per successioni convergenti):

Siano $(a_{n})_{n\in\mathbb{N}}$ e $(b_{n})_{n\in\mathbb{N}}$ successioni di numeri reali. Siano $a,b\in \mathbb{R}$. Supponiamo che $\exists\lim\limits_{ n \to \infty }a_{n}=a$ e $\exists \lim\limits_{ n \to \infty }b_{n}=b$. Allora, valgono le seguenti implicazioni:
1. $a<b\implies a_{n}<b_{n}$ definitivamente
2. $a_{n}\leq b_{n}$ definitivamente $\implies a\leq b$.

*Dimostrazione*:
1. Supponiamo che $a<b$, ossia $b-a>0$. Consideriamo la successione $(a_{n}-b_{n})_{n\in \mathbb{N}}$ è convergente e $\lim\limits_{ n \to \infty }(a_{n}-b_{n})=\lim\limits_{ n \to \infty }(a_{n}+(-b_{n}))=\lim\limits_{ n \to \infty }a_{n}+\lim\limits_{ n \to \infty }(-b_{n})=a-b<0$.
	Quindi, per il teorema della permanenza del segno, si ha che $a_{n}-b_{n}<0$ definitivamente. Ossia $a_{n}<b_{n}$ definitivamente.
2. Supponiamo che $a_{n}\leq b_{n}$ definitivamente e proviamo che $a\leq b$. Se per assurdo fosse $b< a$ allora, per il punto $1)$ avremmo che $b_{n}<a_{n}$ definitivamente, assurdo $\blacksquare$.

*Proposizione*(criterio del confronto per successioni divergenti):
Supponiamo che $(a_{n})_{n\in\mathbb{N}}$ e $(b_{n})_{n\in\mathbb{N}}$ siano successioni di numeri reali. Supponiamo anche che 
1. $a_{n}\leq b_{n}$ definitivamente
2. $\exists \lim\limits_{ n \to \infty }a_{n}=+\infty$
Allora $\exists \lim\limits_{ n \to \infty }b_{n}=+\infty$.
Inoltre, se:
1. $a_{n}\leq b_{n}$ definitivamente
2. $\exists \lim\limits_{ n \to \infty }b_{n}=-\infty$
Allora $\exists \lim\limits_{ n \to \infty }a_{n}=-\infty$.

*Dimostrazione*:
Dimostriamo il primo caso. Supponiamo che valgano $1)$ e $2)$ e verifichiamo che $\exists \lim\limits_{ n \to \infty }b_{n}=+\infty$. Ossia $\forall k>0 \exists \nu \in \mathbb{N}$ tale che $\forall n\in \mathbb{N},\,n\geq \nu: b_{n}>k$. 
Sia $k>0$. Poiché $\exists \lim\limits_{ n \to \infty }a_{n}=+\infty$, in corrispondenza di tale $k$: $$
\exists \nu \in \mathbb{N}, \text{ tale che }\forall n\in\mathbb{N},\,n\geq \nu: a_{n}>k.
$$
Poiché $a_{n}\leq b_{n}$ definitivamente, si ha che: $\exists \tilde{\nu}\in \mathbb{N}$ tale che $\forall n\in \mathbb{N},\,n\geq \tilde{\nu}:k<a_{n}<b_{n}$, quindi $b_{n}>k$ definitivamente.
Si dimostra in maniera analoga l'altro caso $\blacksquare$.

*Teorema*(convergenza obbligata (o dei carabinieri) per successioni):
Siano $(a_{n})_{n\in\mathbb{N}}$, $(b_{n})_{n\in\mathbb{N}}$, $(c_{n})_{n\in\mathbb{N}}$ successioni di numeri reali. Supponiamo che: 
1. $a_{n}\leq b_{n}\leq c_{n}$ definitivamente
2. $\exists \lim\limits_{ n \to \infty }a_{n}=\lim\limits_{ n \to \infty }a_{n}=l\in \mathbb{R}$.
Allora: $$
\exists \lim\limits_{ n \to \infty } b_{n}=l.
$$
*Dimostrazione*:
Vogliamo provare che $\exists \lim\limits_{ n \to \infty }b_{n}=l\in \mathbb{R}$, ossia $\forall\varepsilon>0\exists \nu \in \mathbb{N}$ tale che $\forall n\in \mathbb{N},\,n\geq \nu: |b_{n}-l|<\varepsilon \implies l-\varepsilon<b_{n}<l+\varepsilon$.
Fissiamo $\varepsilon>0$. Poiché $\exists \lim\limits_{ n \to \infty }a_{n}=\lim\limits_{ n \to \infty }c_{n}=l$, in corrispondenza di $\varepsilon>0$ $$
\exists \nu \in \mathbb{N}\text{ tale che } l-\varepsilon<a_{n}<l+\varepsilon \,\wedge\, l-\varepsilon<b_{n}<l+\varepsilon.
$$
Poiché $a_{n}<b_{n}<c_{n}$ definitivamente, si ha, definitivamente, che $$
l-\varepsilon<a_{n}\leq b_{n}\leq c_{n}<l+\varepsilon.
$$
Ossia $l-\varepsilon<b_{n}<l+\varepsilon$ definitivamente $\blacksquare$.
