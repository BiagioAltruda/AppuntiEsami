**Numeri complessi**
*Definizione*:
Sia $n\in \mathbb{N},\, n\geq2$. Si dice radice $n-esima$ del numero complesso $z$ ogni numero complesso $w$ tale che $w^{n}=z$.
*Proposizione* (Formule di de Moivre):
Sia $z$ un numero complesso non nullo, di modulo $\rho$ ed argomento $\vartheta$. Allora $z$ ha esattamente $n$ radici n-esime, date dalle seguenti formule:
$$
\text{Forma Trigonometrica: } x_{k}=\left[ \sqrt[n]{\rho}, \frac{\vartheta+2k\pi}{n} \right], \text{ per } k=0,\dots,n-1;
$$
$$
\text{Forma esponenziale } x_{k}=\sqrt{ \rho }e^{\frac{\vartheta+2k\pi}{n}}= \rho e^{i\vartheta}=z
$$
*Dimostrazione*:
Utilizzeremo la notazione esponenziale. Proviamo che, $\forall k=0,\dots,n-1$, $x_{k}$ è una radice $n-esima$ di $z=\rho e^{i\vartheta}$. In effetti, si ha che:
$$
x_{k}^{n}=\left( \sqrt[n]{ \rho }e^{i \frac{\vartheta+2k\pi}{n} } \right)^{n}= \rho e^{i(\vartheta+2k\pi)} = \rho e ^{i\vartheta}=z 
$$
Proviamo ora che ogni radice $n-esima$ di $z$ è uguale ad uno degli zeri di $x_{k}$. Sia quindi $w$ una radice $n-esima$ di $z$, $w=\sigma e^{i\varphi}.$ Allora si ha che $$
w^{n}=(\sigma e^{i\varphi})^{n}=\sigma^{n}e^{in\phi}=\rho e^{i\vartheta}.
$$
Dall'ultima disuguaglianza che traduce la condizione $w^{n}=z$, segue, confrontando i moduli e gli argomenti secondo il criterio di uguaglianza per le forme trigonometriche:
$$
\begin{cases}
\sigma^{n}=\rho \\ \\
n\varphi=\vartheta+2k\pi & \text{per qualche } k\in \mathbb{Z}
\end{cases}
$$
ossia,
$$
\begin{cases}
\sigma=\sqrt[n]{ \rho } \\ \varphi= \frac{\vartheta+2k\pi}{n} & \text{ per qualche } k\in \mathbb{Z}
\end{cases}
$$
Sia ora $r$ il resto della divisione di $k$ per $n$. Allora $r\in 0,\dots,n-1$, e $k=qn+r$ per un opportune $q\in \mathbb{Z}$. Segue che 
$$
\frac{\vartheta+2k\pi}{n}= \frac{\vartheta+2(qn+r)\pi}{n}= \frac{\vartheta+2r\pi}{n} + 2q\pi. 
$$
Dunque è indifferente prendere, come argomento, $\frac{\vartheta+2k\pi}{n}$ oppure $\frac{\vartheta+2r\pi}{n}$. Segue che 
$$
w=\sigma e^{i\varphi}=\sqrt[n]{ \rho }e^{i \frac{\vartheta+2r\pi}{n}}=x_{r}.
$$
Abbiamo così provato che le formule di De Moivre forniscono tutte le radici $n-esime$ di $z$. Proviamo allora che i numeri $x_{r}$ sono a due a due distinti (ovvero che sono esattamente $n$). Siano quindi $k,k'=0,\dots,n-1$, con $k\neq k'$. Allora gli argomenti di $x_{k}$ e $x_{k'}$ differiscono per il numero $\frac{2(k-k')\pi}{n}= \frac{k-k'}{n}2\pi$, che non è multiplo intero di $2\pi$: infatti
$$
-(n-1)\leq k-k' \leq n-1, \text{ e } k-k'\neq0
$$
per cui $k-k'$ non è divisibile per $n$ e di conseguenza $\frac{k-k'}{n}$ non è un intero. Segue quindi che $x_{k}$ e $x_{k'}$ sono diversi, come voluto $\blacksquare$ .

**Gruppi e sottogruppi**
*Definizione*:
Sia $X$ un insieme non vuoto. Si dice operazione binaria su $X$ ogni applicazione da $X \times X \to X$.
*Definizione*:
Si dice gruppo ogni coppia ordinata $(G,*)$, dove $G$ è un insieme non vuoto e $*$ è un operazione su $G$ verificante le seguenti condizioni:
1. $\forall x,y,z \in G,\, x*(y*z)=(x*y)*z$
2. $\exists e \in G$ tale che $\forall x \in G, \, x*e=e*x=x$
3. $\forall x \in G,\, \exists \bar{x}\in G$ tale che $x* \bar{x}= \bar{x}*x=e$
Il gruppo si dice abeliano o commutativo se vale anche 
4. $\forall x,y\in G,\, x*y=y*x$

*Proposizione*:
Sia $(G,*)$ un gruppo. Allora l'elemento neutro è unico e ogni elemento ha un unico simmetrico.
*Dimostrazione*:
Siano $e_{1},e_{2}$ elementi neutri per $G$. Allora si ha
$$
e_{1}=e_{1}*e_{2}=e_{2}\,\,\blacksquare.
$$
Sia adesso $x \in G$ e siano $x_{1},x_{2}$ due suoi simmetrici. Sia $e$ il neutro di $G$. Allora si ha:
$$
x_{1}=x_{1}*e=x_{1}*(x*x_{2})=(x*x_{1})*x_{2}=e*x_{2}=x_{2} \,\, \blacksquare.
$$
*Proposizione*:
Sia $(G,*)$ un gruppo. Allora
1. $\forall x \in G,\, \bar{\bar{x}}=x$
2. $\forall x,y\in G, \bar{x*y}= \bar{y}*\bar{x}$
*Dimostrazione*:
$1)$ è immediata conseguenza della definizione di sopra.
Mentre per $2)$: siano $x,y\in G$. Sia $e$ l'elemento neutro di $G$. Allora si ha:
$$
(x*y)*(\bar{y}*\bar{x})=x*(y*(\bar{y}*\bar{x}))=x*((y*\bar{y})*\bar{x})=x*(e*\bar{x})= x *\bar{x}=e
$$
La prima e la seconda uguaglianza derivano dall'associatività, la terza dal fatto che $\bar{y}$ è il simmetrico di $y$, la quarta dal fatto che $e$ è l'elemento neutro di $G$, l'ultima dal fatto che $\bar{x}$ è il simmetrico di $x$. Analogamente si prova che 
$$
(\bar{y}*\bar{x})*(x*y)=e \,\, \blacksquare.
$$
*Proposizione*:
Sia $(G,*)$ un gruppo. Allora $\forall x,y,z\in G$ valgono le seguenti implicazioni:
1. $x*y=x*z \implies y=z$
2. $y*x=z*x \implies y=z$
*Dimostrazione*:
Proviamo $1)$, l'altra è analoga. Siano quindi $x,y,z\in G$. Allora valgono le seguenti implicazioni:
$$
x*y=x*z \implies \bar{x}*(x*y)=\bar{x}*(x*z) \implies y=z\,\,\blacksquare.
$$
*Definizione*:
Sia $(G,*)$ un gruppo, e sia $H$ un sottoinsieme non vuoto di $G$. Si dice che $H$ è chiuso rispetto all'operazione $*$ se, $\forall x,y\in H,\,x*y\in H$.

*Definizione*:
Sia $(G,*)$ un gruppo, e sia $H$ un sottoinsieme non vuoto di $G$, chiuso rispetto all'operazione $*$. Si dice operazione $*$ ristretta ad $H$ l'operazione $*_{H}$ su $H$ così definita: $\forall x,y\in H, \, x*_{H}y=x*y$.

*Definizione*:
Sia $(G,*)$ un gruppo e sia $H$ un sottoinsieme non vuoto di $G$. Allora $H$ si dice un sottogruppo di $G$ se:
1. $H$ è chiuso rispetto all'operazione $*$
2. $H$ è un gruppo rispetto all'operazione $*$ ristretta.
In tal caso si scrive anche $H<G$.

*Proposizione*:
Sia $(G,*)$ un gruppo e sia $H$ un suo sottogruppo. Allora:
1. l'elemento neutro di $H$ è l'elemento neutro di $G$.
2. Il simmetrico in $H$ di ogni suo elemento è il suo simmetrico in $G$.
*Dimostrazione*:
$1)$ Sia $e$ il neutro di $H$. Allora $e$ è un elemento idempotente del gruppo $H$ e dunque $e=e*_{H}e=e*e$. Ma allora $e$ è un elemento idempotente del gruppo $G$. Segue che $e$ è l'elemento neutro anche di $G$.
$2)$ Sia $x$ un elemento di $H$, e sia anche $\bar{x}$ il suo simmetrico in $H$. Allora $x*\bar{x}=\bar{x}*x=e$. Poiché questo è l'elemento neutro di $G$ segue che $\bar{x}$ è il simmetrico di $x$ in $G$.

*Proposizione*:
Sia $(G,*)$ un gruppo, e sia $H$ un sottoinsieme non vuoto di $G$. Allora sono equivalenti le seguenti condizioni:
1. $H$ è sottogruppo di $G$
2. $\forall x,y\in H, x*\bar{y}\in H$

*Dimostrazione*:
Proviamo che $1)\implies2)$. Sia $H$ un sottogruppo di $G$ e siano $x,y,\in H$. Allora $\bar{y}\in H$. Essendo inoltre $H$ chiuso per l'operazione $*$ si ha che $x*\bar{y}\in H$.
Adesso $2)\implies 1)$. Sia $e$ l'elemento neutro di $G$. Essendo $H$ non vuoto, esiste $x \in H$. Allora, per ipotesi, $e=x*\bar{x}\in H$. Ma come abbiamo appena visto $\bar{x}=e*\bar{x}\in H$. Siano adesso $x,y\in H$. Allora come abbiamo appena verificato, $\bar{y}\in H$ e, pertanto, $x*y=x*\bar{\bar{y}}\in H$.

*Corollario*:
Sia $(G,*)$ un gruppo e siano $H,K$ due suoi sottogruppi. Allora anche $H\cap K$ è un sottogruppo di $G$.

*Dimostrazione*:
Sia $e$ l'elemento neutro di $G$, si ha che $e\in H$ ed $e\in K$ allora $e\in H\cap K$. In particolare l'intersezione è non vuota. Siano adesso $x,y\in H\cap K$, e quindi $x*\bar{y}\in H$ ma anche $x*\bar{y}\in K$ allora $x*\bar{y}\in H\cap K$ come voluto.

*Corollario*:
Ogni sottogruppo di un gruppo abeliano, è abeliano.

--------
**Omomorfismi di Gruppi**
*Definizione*:
Siano $(G_{1},*_{1})$ e $(G_{2},*_{2})$ gruppi. un'applicazione $f:G_{1}\to G_{2}$, si dice un omomorfismo di gruppo se, $\forall x,y\in G_{1}$,
$$
f(x*_{1}y)=f(x)*_{2}f(y).
$$
Se $(G_{1},*_{1}),(G_{2},*_{2})$ sono uguali, $f$ si dice endomorfismo. Un omomorfismo bigettivo si dice isomorfismo. Un endomorfismo bigettivo si dice automorfismo.

*Proposizione*:
Siano $(G_{1},*_{1})$ e $(G_{2},*_{2})$ gruppi, e sia $f:G_{1}\to G_{2}$ un omomorfismo di gruppi. Allora valgono le seguenti proprietà:
1. $f(e_{1})=e_{2}$
2. $\forall x \in G_{1},\overline{f(x)}=f(\bar{x})$
3. Se $H<G_{1}$, allora $f(H)<G_{2}$
4. Se $H<G_{2}$, allora $f^{-1}(H)<G_{1}$.
*Dimostrazione*:
1. Si ha $f(e_{1})=f(e_{1}*_{1}e_{1})=f(e_{1})*_{2}f(e_{1})$, per cui $f(e_{1})$ è idempotente in $G_{2}$ e quindi è l'elemento neutro.
2. Sia $x \in G_{1}$. Allora si ha: $$
e_{2}=f(e_{1})=f(x*_{1}\bar{x})=f(x)*_{2}f(\bar{x})
$$
$$
e_{2}=f(e_{1})=f(\bar{x}*_{1}x)=f(\bar{x})*_{2}f(x)
$$
Segue che $f(\bar{x})$ è il simmetrico di $f(x)$.
3. Sia $H_{1}<G_{1}$. Allora $e_{1}\in H_{1}$. In particolare $f(H_{1})\neq \emptyset$. Siano allora $x,y\in H_{1}$. Per la caratterizzazione dei sottogruppi abbiamo che $x*_{1}\bar{y}\in H$, quindi: $$
f(x)*_{2}\overline{f(y)}=f(x)*_{2}f(\bar{y})= f(x*_{1}\bar{y})\in f(H_{1}),
$$
	Il che prova che $f(H_{1})$ è un sottogruppo di $G_{2}$.
4. Sia $H_{2}<G_{2}$. Allora, per quanto già dimostrato prima $e_{1}\in f^{-1}(H_{2})$. In particolare $f^{-1}(H_{2})$ è non vuoto. Siano quindi $x,y\in f^{-1}(H_{2})$. Allora $f(x),f(y)\in H_{2}$. Abbiamo che: $$
f(x*_{1}\bar{y}=f(x)*_{2}f(\bar{y}))=f(x)*_{2}\overline{f(y)}\in H
$$
Pertanto $x*_{1}\bar{y}\in f^{-1}(H_{2})$ che prova che $f^{-1}(H)<G_{1}$.

*Definizione*:
Siano $(G_{1},*_{1}),(G_{2},*_{2})$ gruppi. Sia $f:G_{1}\to G_{2}$ un omomorfismo di gruppi. Allora si dice nucleo di $f$, l'insieme $$
Kerf= f^{-1}(e_{2})=\left\{ x \in G|\, f(x)=e_{2} \right\} 
$$
Mentre si dice immagine di $f$ l'insieme: $$
\mathrm{Im}f=f(G_{1})=\left\{ f(x)|\,x \in G_{1} \right\} 
$$

*Corollario*:
Siano $G_{1}$ e $G_{2}$ gruppi, come prima. Sia $f:G_{1}\to G_{2}$ un omomorfismo di gruppi. Allora $Kerf$ è un sottogruppo di $G_{1}$ ed $\mathrm{Im}f$ è un sottogruppo di $G_{2}$

*Definizione*: Si dice monomorfismo un omomorfismo iniettivo. Si dice epimorfismo un omomorfismo suriettivo.

*Osservazione*:
Un omomorfismo è un isomorfismo se e solo se è sia un monomorfismo che un epimorfismo.

*Proposizione*:
Siano $(G_{1},*_{1})$ e $(G_{2},*_{2})$ gruppi e sia $f:G_{1}\to G_{2}$ un omomorfismo di gruppi. Allora:
1. f è un monomorfismo se e solo se $Kerf=\left\{ 0 \right\}$
2. f è un epimorfismo se e solo se $\mathrm{Im}f=G_{2}$.
*Dimostrazione*:
1. $e_{1}\in Kerf$. Supponiamo che $f$ sia iniettivo. Se $x \in Kerf$ allora $f(x)=e_{1}=f(e_{1})$. Dall'iniettività segue che $x=e_{1}$. Viceversa supponiamo che $Kerf=\left\{ e_{1} \right\}$. Siano $x,y\in G$ tali che $f(x)=f(y)$, allora: $$
e_{2}=f(x)*_{2}\overline{f(y)}=f(x)*_{2}f(\bar{y})=f(x*_{1}\bar{y}).
$$
	Dunque $x*_{1}\bar{y}\in Kerf$. Che implica che $x*_{1}\bar{y}=e_{1}$. Dunque $x=y$. Quindi $f$ è un monomorfismo
2. La tesi segue immediatamente dalle definizioni.

*Notazione*:
D'ora in poi, a meno che non sia particolarmente ambiguo, smetterò di differenziare le varie operazioni dei gruppi (soprattutto durante i conti) per non appesantire la notazione.

*Proposizione*:
Siano $(G_{1},*_{1}), (G_{2},*_{2})$ e $(G_{3},*_{3})$ gruppi e siano $f:G_{1}\to G_{2}$ e $g:G_{2}\to G_{3}$ omomorfismi di gruppi. Allora $g \circ f:G_{1}\to G_{3}$ è un omomorfismo di gruppi.

*Dimostrazione*:
Siano $x,y\in G_{1}$. Allora
$$
g \circ f(x*y)=g(f(x)*f(y)))=g(f(x))*g(f(y))=g\circ f(x) * g\circ f(y).
$$
Come richiesto.

*Proposizione*:
L'applicazione inversi di un isomorfismo di gruppi è un isomorfismo di gruppi.

*Dimostrazione*:

Siano $(G_{1},*_{1})$ e $(G_{2},*_{2})$ gruppi e sia $f:G_{1}\to G_{2}$ un isomorfismo di gruppi. Sia anche $f^{-1}:G_{2}\to G_{1}$ la sua applicazione inversa. Poiché essa è bigettiva, resta da provare che essa è un omomorfismo. Siano $u,v\in G_{2}$ e siano $x=f^{-1}(u)$ e $y=f^{-1}(v)$. Allora, essendo $f$ un omomorfismo vale:
$$
f(x*y)=f(x)*f(y)=f(f^{-1}(u))* f(f^{-1}(v))=u*v
$$
Segue:
$$
f^{-1}(u*v)=x*y=f^{-1}(u)*f^{-1}(v).
$$
Ciò prova che $f^{-1}$ è un omomorfismo e dunque un isomorfismo.

*Definizione*:
Si dice che il gruppo $(G_{1},*_{1})$ è isomorfo al gruppo $(G_{2},*_{2})$ se esiste un isomorfismo di gruppi $f:G_{1}\to G_{2}$. In tal caso si scrive $G_{1} \simeq G_{2}$.

Come spiegato nella prossima proposizione, la relazione tra gruppi di essere isomorfi è una relazione di equivalenza.

*Proposizione*:
La relazione di isomorfismo tra gruppi è riflessiva, simmetrica e transitiva.

*Proposizione*:
Siano $(G_{1},*_{1})$ e $(G_{2},*_{2})$ gruppi isomorfi. Allora $G_{1}$ è abeliano se e solo se lo è anche $G_{2}$.

*Dimostrazione*:
Sia $f:G_{1}\to G_{2}$ un isomorfismo di gruppi. Supponiamo che $G_{1}$ sia abeliano. Siano $u,v\in G_{2}$. Siano $x=f^{-1}(u)$ e $y=f^{-1}(v)$. Allora:
$$
u*v=f(x)*f(y)=f(x*y)=f(y*x)=f(y)*f(x)=v*u
$$
Invertendo i ruoli di $G_{1}$ e $G_{2}$ si prova l'implicazione opposta.

**Gruppi di permutazioni**
Sia $X$ un insieme non vuoto. Si dice permutazione su $X$ ogni applicazione bigettiva da $X$ in se stesso. Denoteremo con $S(X)$ l'insieme delle permutazioni su $X$.

*Proposizione*:
L'insieme $S(X)$ è un gruppo rispetto alla composizione di applicazioni.

*Dimostrazione*:
La composizione di due permutazioni di $X$ è ancora una permutazione di $X$, infatti: se $f:X\to X$ e $g:X\to X$ sono bigezioni, bigettiva è anche l'applicazione composta $g \circ f:X\to X$. Quindi la composizione di applicazioni è un'operazione binaria su $S(X)$.
L'associatività è nota dalla teoria delle applicazioni. L'elemento neutro è l'applicazione identica $id_{X}$. Infine $\forall f\in S(X)$, l'applicazione inversa $f^{-1}$ appartiene anch'essa a $S(X)$ dato che $f \circ f^{-1}=f^{-1}\circ f= id_{X}$. Essa è quindi il simmetrico di $f$ in $S(X)\,\blacksquare$.

*Definizione*:
Sia $n\in \mathbb{N}$, ed $X=\left\{ 1,2,\dots,n \right\}$. Allora il gruppo $S(X)$ viene detto gruppo simmetrico su $n$ elementi. Si denota con $S_{n}$ oppure con $Sym(n)$.

*Proposizione*:
$\forall n\in \mathbb{N}$, $S_{n}$ ha esattamente $n!$ elementi.

*Dimostrazione*:
Il numero di elementi di $S_{n}$ è pari al numero di disposizioni di $n$ numeri interi.
Dimostriamo la tesi per induzione su $n$. La tesi è chiaramente vera per $n=1$. Sia ora $n>1$ e supponiamo la tesi vera per $n-1$. Ogni disposizione di $n$ numeri si ottiene scegliendo uno dei numeri come il primo ed occupando le posizione restanti con gli $n-1$ numeri non ancora scelti. Queste ultime per ipotesi induttiva sono $(n-1)!$, mentre le possibili scelte per il primo numero sono $n$. Quindi complessivamente ho $n(n-1)= n!$ possibili scelte $\blacksquare$.

*Proposizione*:
$S_{n}$ è abeliano se e solo se $n\leq 2$.

*Dimostrazione*:
Basta provare che per ogni $x\geq 3$, $S_{n}$ non è abeliano. Sia quindi $n\geq 3$, e siano $\sigma,\tau \in S_{n}$ così definiti:
$$
\sigma(1)=2, \sigma(2)=1, \forall i \neq 1,2: \sigma(i)=i
$$
$$
\tau(1)=3, \tau(3)=1, \forall i\neq 1,3: \tau(i)=i
$$
Allora $\sigma \circ \tau(1)=\sigma (3)=3$, mentre $\tau \circ \sigma (1)=\tau(2)=2\, \blacksquare$.

*Osservazione*:
Sia $n\geq 2$ un intero. Per ogni polinomio $p(x_{1},\dots,x_{n})$ a coefficienti nelle indeterminate $x_{1},\dots,x_{n}$, poniamo $\sigma(p)=p(x_{\sigma(1)},\dots,x_{\sigma(n)})$

Consideriamo il polinomio
$$
p_{n}=\prod_{1\leq i<j\leq n}(x_{i}-x_{j})
$$
Allora
$$
\sigma(p_{n})=\prod_{1\leq i<j\leq n}(x_{\sigma(i)}-x_{\sigma(j)})
$$
In particolare: $p_{n}$ e $\sigma(p_{n})$ differiscono al più per un segno.

*Definizione*:
Una permutazione $\sigma \in S_{n}$ si dice (di segno o di classe) pare se $\sigma(p_{n})=p_{n}$. Altrimenti si dice dispari.

*Osservazione*:
Dal fatto che $s$ è un omomorfismo di gruppi si deduce la seguente regola di composizione per le permutazioni pari e dispari:
1. Se $\sigma,\tau \in S_{n}$, hanno lo stesso segno allora $\sigma\circ \tau$ è pari;
2. altrimenti $\sigma\circ \tau$ è dispari.

*Proposizione*:
Sia $n$ un intero positivo. L'insieme delle permutazioni pari di $S_{n}$ è un sottogruppo detto $A_{n}$.

*Proposizione*:
$\forall n\geq 2,\, A_{n}$ ha ordine $\frac{n!}{2}$.

*Dimostrazione*:
Sia $n\geq 2$. Sia $B_{n}$ l'insieme delle permutazioni dispari di $S_{n}$. Allora si ha che $S_{n}=A_{n}\cup B_{n}$, in particolare l'unione è disgiunta e quindi:
$$
|S_{n}|=|A_{n}|+|B_{n}|.
$$
Sia $\alpha \in S_{n}$ la permutazione: $\alpha(1)=2,\,\alpha(2)=1,\,\alpha(i)=i,\, \forall i=3,\dots,n$, una permutazione dispari.
Definiamo l'applicazione $\varphi:A_{n}\to B_{n}$, ponendo $\varphi(\sigma)=\sigma\circ \alpha,\, \forall \sigma \in A_{n}$. $\varphi$ è un'applicazione ben definita. Notiamo che essendo $\alpha$ dispari, allora anche $\sigma\circ\alpha$ lo è. Proviamo che $\varphi$ è invertibile. Sia $\psi:B_{n}\to A_{n}$ l'applicazione definita ponendo $\psi(\sigma)=\sigma\circ \alpha,\, \forall \sigma \in B_{n}$. Anche $\psi$ è ben definita. Si ha che $\forall \sigma \in A_{n}$,
$$
\psi \circ \varphi(\sigma)=\psi(\varphi(\sigma))=\psi(\sigma\circ \alpha)= (\sigma \circ \alpha)\circ \alpha= \sigma \circ (\alpha\circ\alpha)=\sigma\circ id= \sigma
$$
Quindi le applicazioni $\psi$ e $\varphi$ sono l'una l'inversa dell'altra, ed essendo bigezioni, segue che $|A_{n}|=|B_{n}|$. Ovvero $|A_{n}|=\frac{|S_{n}|}{2}=\frac{n!}{2}$.

**Anelli**
*Definizione*:
Si dice anello ogni terna ordinata $(A,+,\cdot)$, dove $A$ è un insieme non vuoto e $+$ e $\cdot$ sono operazioni binarie su $A$ verificanti le seguenti condizioni:
1. $(A,+)$ è un gruppo abeliano
2. $\forall a,b,c\in A a\cdot(b\cdot c)=(a\cdot b)\cdot c$
3. $\forall a,b,c\in A,\, a\cdot(b+c)= a\cdot b+a\cdot c$ e $(b+c)\cdot a= b\cdot a + c\cdot a$.

L'anello si dice commutativo se lo è il prodotto.
L'anello si dice unitario se esiste un elemento neutro del prodotto.

*Proposizione*:
Sia $A$ un anello. Allora vale che:
1. $\forall a\in A,\, a 0=0 a=0$.
2. $\forall a,b\in A,\,(-a)b=a(-b)=-ab,\, (-a)(-b)=ab$.
3. Se l'anello $A$ è unitario allora l'elemento $1$ è unico.

*Dimostrazione*:
1. $\forall a\in A$:
$$
a0= a(0+0)=a 0 + a 0,
$$
	Segue che $a 0$ è idempotente in $A$, allora $a 0$ è l'elemento neutro della somma su $A$.
2. $\forall a,b\in A$
$$
(-a)b +ab= (-a+a)b=0
$$
	ciò prova che $(-a)b$ è l'opposto di $ab$ in $(A,+)$. Per l'unicità dell'opposto otteniamo che $(-a)b=a(-b)=-ab$
3. Siano $1$ e $1'$ elementi neutri del prodotto dell'anello unitario $A$. Allora $1=11'=1' \,\blacksquare$.

*Definizione*:
Sia $A$ un anello unitario. Un elemento $a$ di $A$ si dice invertibile a destra se $\exists u\in A$ tale che $au=1$. $u$ si dice inverso destro di $a$. Idem per invertibile a sinistra.

*Proposizione*:
In un anello unitario, un elemento è invertibile se e solo se è invertibile sia a destra che a sinistra. In questo caso l'inverso è unico, ed è anche l'unico inverso destro e sinistro.

*Dimostrazione*:
Sia $A$ un anello unitario e sia $a\in A$. Se $a$ è invertibile, allora, se $w$ è l'inverso di $a$, $w$ è anche inverso destro e sinistro di $a$. Viceversa supponiamo che $a$ ammetta $u$, un suo inverso destro e $v$, un suo inverso sinistro. Allora si ha:
$$
u=1\cdot 1= (va)u=v(au)=v\cdot1=v\, \blacksquare.
$$
*Proposizione*:
L'insieme degli elementi invertibili di un anello unitario, munito della restrizione del del prodotte dell'anello, è un gruppo moltiplicativo.

*Dimostrazione*:
Sia $A$ un anello unitario, e sia $U$ l'insieme dei suoi elementi invertibili. Allora $U$ è chiuso rispetto al prodotto di $A$: infatti, $\forall a,b\in U$, si ha che $b^{-1}a^{-1}$ è l'inverso di  $ab$, e quindi $ab\in U$. Proviamo ora che rispetto a quest'operazione $U$ è un gruppo. La proprietà associativa è chiaramente verificata. L'esistenza degli inversi è anch'essa assicurata per costruzione.

*Definizione*:
L'insieme degli elementi invertibili di un anello $A$ si dice gruppo delle unità di $A$, si denota con $\mathcal{U}(A)$.

*Definizione*:
Un anello unitario, non ridotto ad un singolo elemento, in cui ogni elemento non nulla è invertibile si dice corpo. Un corpo commutativo si chiama campo.

*Definizione*:
Sia $A$ un anello e sia $a\in A, \,a \neq0$. Allora $a$ si dice essere un divisore dello zero se $\exists b\in A,\,b\neq 0$ tale che $ab=0$ oppure $ba=0$. Altrimenti $a$ si dice regolare.

*Definizione*:
Un anello si dice integro se non contiene divisori dello zero.
Un anello commutativo unitario integro e non banale si chiama dominio d'integrità

*Osservazione*:
Un anello $A$ è integro se e solo se in esso vale la legge di annullamento del prodotto.

*Proposizione*:
In un anello unitario non nullo, ogni elemento invertibile è regolare.

*Dimostrazione*:
Sia $A$ un anello unitario non nulla e sia $a\in A$ invertibile. Allora $a\neq 0$. Sia anche $b\in A$ tale che $ab=0$ oppure $ba=0$. Nel primo caso avremmo che $0=a^{-1}0=a^{-1}(ab)=(a^{-1}a)b=b$. Ciò dimostra che non esiste per $a$ un elemento $b$ diverso da $0$ il cui prodotto fa $0\,\blacksquare$.

*Definizione*:\
Sia $A$ un anello e sia $a\in A$. Allora $a$ si dice cancellabile a destra se, $\forall x,y\in A,\,xa=ya\implies x=y$. Analogamente si definiscono gli elementi cancellabili a sinistra.

*Proposizione*:
