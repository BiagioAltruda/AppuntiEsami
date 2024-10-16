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
In un anello, un elemento non nullo è regolare se e solo se è cancellabile.

*Dimostrazione*:
Sia $A$ un anello. Sia $a\in A,\,a\neq 0$. Supponiamo che $a$ sia regolare. Siano $x,y\in A$. Tali che $xa=ya$. Allora, per la proprietà distributiva otteniamo:
$$
0=xa-ya=xa+(-ya)=xa+(-y)a=(x-y)a
$$
Essendo $a$ regolare si deve avere che $x=y$. Quindi $a$ è cancellabile a destra. Analogamente si prova che $a$ è cancellabile a sinistra.
Supponiamo che $a$ sia cancellabile. Sia quindi $b\in A$ tale che $ab=0$ o $ba=0$. Nel primo caso avremmo $ab=a0$. Essendo $a$ cancellabile a sinistra, segue che $b=0$. Si arriva alla stessa conclusione anche nell'altro caso. Segue immediatamente che $a$ è regolare.

*Definizione*:
Sia $(A,+,\cdot)$ un anello, e sia $B$ un sottoinsieme non vuoto di $A$. Allora $B$ si dice un sottoanello di $A$ se:
1. $B$ è chiuso rispetto alle operazioni $+$ e $\cdot$
2. $B$ è un anello rispetto alla restrizione delle operazioni di sopra

Seguono due caratterizzazioni dei sottoanelli.

*Proposizione* :
Sia $A$ un anello, e sia $B$ un suo sottoinsieme non vuoto. Allora $B$ è sottoanello se e solo se:
1. $B$ è sottogruppo additivo di $A$.
2. $B$ è chiuso rispetto al prodotto di $A$.

*Corollario*:
Sia $A$ un anello, e sia $B$ un suo sottoinsieme non vuoto. Allora $B$ è sottoanello se e solo se:
1. $\forall a,b\in B, a-b\in B$;
2. $B$ è chiuso rispetto al prodotto di $A$.

*Proposizione*:
Ogni sottoanello di un anello commutativo è commutativo.

*Dimostrazione*:
credici

*Proposizione*:
Sia $A$ un anello unitario. Se $B$ è un sottoanello di $A$ tale che $1\in B$, allora $\mathcal{U}(B)$ è un sottogruppo di $\mathcal{U}(A)$.

*Definizione*:
Sia $(K,+,\cdot)$ un corpo (o campo), e sia $L$ un sottoinsieme non vuoto di $K$. Allora $L$ si dice sottocorpo (sottocampo) se:
1. $L$ è chiuso rispetto a $+$ e $\cdot$
2. $L$ è un corpo (campo) rispetto alle operazioni ristrette.

*Definizione*:
Siano $(A_{1},+_{1},\cdot_{1})$ e $(A_{2},+_{2},\cdot_{2})$ anelli. Un'applicazione $f:A_{1}\to A_{2}$ si dice omomorfismo di anelli se, $\forall a,b\in A$:
$$
f(a+b)=f(a)+f(b)
$$
$$
f(a\cdot b)= f(a) \cdot f(b)
$$
*Proposizione*:
Siano $(A_{1},+_{1},\cdot_{1})$ e $(A_{2},+_{2},\cdot_{2})$ anelli e sia $f:A_{1}\to A_{2}$ un omomorfismo di anelli. Allora valgono:
1. Se $B_{1}$ è sottoanello di $A_{1}$ allora $f(B_{1})$ è sottoanello di $A_{2}$
2. Se $B_{2}$ è sottoanello di $A_{2}$, allora $f^{-1}(B_{2})$ è sottoanello di $A_{1}$.

*Definizione*:
Siano $(A_{1},+_{1},\cdot_{1})$ e $(A_{2},+_{2},\cdot_{2})$ anelli e sia $f:A_{1}\to A_{2}$ un omomorfismo di anelli. Allora il nucleo di $f$ è l'insieme:
$$
Kerf=f^{-1}(\left\{ 0 \right\} )=\left\{ a\in A|\,f(a)=0 \right\} 
$$
Si dice immagine di $f$ l'insieme:
$$
\mathrm{Im}f=f(A_{1})=\left\{ f(a)|a\in A_{2} \right\} 
$$
*Corollario*:
Siano $(A_{1},+_{1},\cdot_{1})$ e $(A_{2},+_{2},\cdot_{2})$ anelli e sia $f:A_{1}\to A_{2}$ un omomorfismo di anelli. Allora $Kerf$ è $\mathrm{Im}f$ sono sottoanelli rispettivamente di $A_{1}$ e $A_{2}$.

*Proposizione*:
Siano $(A_{1},+_{1},\cdot_{1})$ e $(A_{2},+_{2},\cdot_{2})$ anelli e sia $f:A_{1}\to A_{2}$ un omomorfismo di anelli. Allora:
1. $f$ è un monomorfismo se e solo se $Kerf=\left\{ 0 \right\}$
2. $f$ è un epimorfismo se e solo se $\mathrm{Im}f=\left\{ A_{2} \right\}$.

*Proposizione*: Siano $(A_{1},+_{1},\cdot_{1})$ e $(A_{2},+_{2},\cdot_{2})$ anelli e sia $f:A_{1}\to A_{2}$ un epimorfismo di anelli. Allora se $A_{1}$ è unitario, anche $A_{2}$ lo è, e $f(1)=1$. Inoltre se $a\in A_{1}$ è invertibile lo è anche $f(a)$ e $f(a)^{-1}=f(a^{-1})$.

*Dimostrazione*:
Sia $a\in A_{2}$. Poiché $f$ è surgettivo, esiste $b\in A$ tale che $f(b)=a$. Allora:
$$
a=f(b)=f(b\cdot1)=f(b)f(1)=af(1)
$$
$$
a=f(b)=f(1\cdot b)= f(1)f(b)=f(1)a
$$
Che dimostra la prima metà.
Essendo $a$ invertibile in $A_{1}$, ed essendo $f$ un epimorfismo vale:
$$
f(a\cdot a^{-1})=f(a) f(a^{-1}) \implies f(1)= f(a)f(a^{-1})\implies 1= f(a)f(a^{-1})
$$
ovvero
$$
f(a^{-1})=f(a)^{-1}.
$$

*Proposizione*:
Valgono per gli anelli le stesse proposizioni sulla composizione di omomorfismi e proprietà di isomorfismi.

----
**Divisibilità, teorema di divisione euclidea e algoritmo delle divisioni successive**

*Definizione*:
Sia $A$ un anello commutativo, e siano, $a,b\in A$. Si dice che $b$ divide $a$ se $\exists q\in A$ tale che $a=bq$. In tal caso si scrive $b|a$.

*Osservazione*:
La divisibilità definisce su un anello commutativo $A$ una relazione transitiva.

*Definizione*:
Sia $A$ un anello commutativo, e siano $a,b\in A$. Allora $a$ e $b$ si dicono associati se $a$ divide $b$ e $b$ divide $a$.

*Proposizione*:
Sia $A$ un dominio di integrità, siano $a,b\in A$. Allora $a$ e $b$ sono associati se e solo se esiste un elemento invertibile $u\in A$ tale che $b=au$.

*Dimostrazione*:
Siano $a$ e $b$ associati. Allora esistono $q,q'\in A$ tali che $a=bq$ e $b=aq'$, da cui $b=(bq)q'=b(qq')$. Se $b$ è zero, allora, anche $a$ è zero, dunque la tesi è verificata per $u=1$. Altrimenti $b$ è un elemento regolare e quindi cancellabile. Allora essendo $b 1=b(qq')$, segue che $1=qq'$. quindi $q$ è invertibile $\blacksquare$.

*Corollario*:
In un anello commutativo unitario, due elementi sono associati se e solo se hanno gli stessi divisori e multipli.

*Proposizione*:
Sia $a$ un anello commutativo. Allora $\forall a,b,c\in A$:
1. se $a|b$ e $a|c$, allora $a| b\pm c$
2. se $a|b$ e $a|b+c$, allora $a|c$
3. se $a|b$, allora $a|bc$.

*Dimostrazione*:
1. Se $a|b,c$, allora esistono $q,q'\in A$ tali che $b=aq,\,c=aq'$, per cui, per la proprietà distributiva, si ha che $b+c=aq+aq'=a(q+q')$, quindi $a$ divide $b+c$. Allo stesso modo si mostra che $a$ divide $b-c$.
2. Basta applicare $1)$ osservando che $c=(b+c)-b$.
3. Se $b=aq$, con $q\in A$, allora $bc=(aq)c=a(qc)$ e quindi $a$ divide $bc$.

*Teorema*(di divisione euclidea):
Sia $a,b\in \mathbb{Z}$, ove $b \neq0$. Allora esistono, e sono univocamente determinati $q,r\in \mathbb{Z}$ tali che:
1. $a=bq+r$;
2. $0\leq r<|b|$
$q$ ed $r$ si dicono rispettivamente quoziente e resto della divisione euclidea di $a$ per $b$.

*Dimostrazione*:
$SPG$ $b>0$. Consideriamo l'insieme:
$$
X=\left\{ a-bx\geq 0| x \in \mathbb{Z} \right\} 
$$
$X$ è non vuoto. Infatti se $a\geq 0$, allora $0\leq a= a- b0 \in X$. Altrimenti essendo $b\geq 1$, si ha $0\leq (1-b)a$. Essendo $X\subset \mathbb{N}$, per il principio del minimo, $\exists r\in X$ tale che $r$ è il suo minimo. Allora, per qualche $q\in \mathbb{Z},\,r=a-bq\geq0$. Vale quindi $1)$. Resta da verificare che $r<|b|$, ossia $r<b$. Supponiamo per assurdo che $r\geq b$. Allora $0\leq r-b=q-b(q+1)$. Quindi $r-b\in X$, pur essendo $r-b<r=\min X$, assurdo. Supponiamo ora che sia $b<0$. Allora $-b>0$ e quindi esistono, come appena dimostrato, $q,r\in \mathbb{Z}$ tali che si abbia $a=-bq+r$ e $0\leq r<|-b|=|b|$.
Proviamo ora l'unicità. Siano $q_{1},q_{2},r_{1},r_{2}\in \mathbb{Z}$ tali che $q=q_{i},r=r_{i}$ con $i=1,2$. Allora:
$$
bq_{1}+r_{1}=bq_{2}+r_{2} \implies b(q_{1}-q_{2})=r_{2}-r_{1}
$$
$SPG$ supponiamo $r_{2}\geq r_{1}$.
$$
|b_{1}||q_{1}-q_{2}|=|b(q_{1}-q_{2})|=r_{2}-r_{1}<|b|
$$
Ma allora $0\leq|q_{1}-q_{2}|<1$, e quindi essendo $q_{1}-q_{2}$ intero segue che $|q_{1}-q_{2}|=0$, cioè $q_{1}=q_{2}$. Segue immediatamente che $r_{1}=r_{2} \, \blacksquare$.

*Definizione*:
Siano $a,b\in \mathbb{Z}$. Allora si dice massimo comune divisore di $a$ e $b$ ogni numero $d$ tale che:
1. $d|a$ e $d|b$
2. $\forall e\in \mathbb{Z}$ tale che $e|a$ e $e|b$, si ha che $e|d$

*Corollario*:
Siano $a,b\in \mathbb{Z}$. Allora $b|a$ se e solo se $b$ è il massimo comun divisore tra $a$ e $b$. Se $a=0$, un massimo comune divisore di $a$ e $b$ è $b$.

*Proposizione* (Lemma di Bézout):
Siano $a,b\in \mathbb{Z}$. Allora esiste un massimo comun divisore $d$ di $a$ e $b$. Inoltre esistono $s,t\in \mathbb{Z}$ tali che:
$$
sa+tb=d
$$
Tale uguaglianza si dice identità di Bézout. I numeri $s,t$ sono i coefficienti di Bézout di $a$ e $b$.

*Dimostrazione*:
Se $a=b$, allora $b$ è un massimo comune divisore di $a$ e $b$, e si possono scegliere $s=0$ e $t=1$. Supponiamo quindi $a$ non nullo. Sia
$$
X=\left\{ ax+by>0|\,x,y\in \mathbb{Z} \right\}.
$$
Allora $X$ è un sottoinsieme di $\mathbb{N}$. $X$ è non vuoto. Per il principio del minimo, $X$ ammette minimo $m$. Siano $s,t\in \mathbb{Z}$ tali che $as+bt=m$. Proviamo che $m$ è un massimo comune divisore di $a$ e $b$. Per provare che $m$ divide $a$ e $b$, utilizziamo il teorema di divisione euclidea. Siano $q$ ed $r$ quoziente e resto della divisione euclidea di $a$ per $m$. Allora $r<m$ e 
$$
r=a-mq=a-(as+bt)q=a(1-sq)+b(-tq).
$$
Se fosse $r>0$, allora si avrebbe che $r\in X$, e quindi $m\leq r$, che è assurdo. Quindi $r=0$, che prova che $m$ divide $a$. Analogamente si prova che $m$ divide $b$. Supponiamo ora che $e\in \mathbb{Z}$ sia tale che $e|a$ e $e|b$. Allora $e|as$ e $e|bt$ e quindi $e|as+bt=m$. Ciò prova che $m$ soddisfa la definizione di sopra, ed è dunque il massimo comune divisore tra $a$ e $b \,\blacksquare$.

*Proposizione*:
Siano $a,b\in \mathbb{Z}$ e sia $d$ un massimo comune divisore di $a$ e $b$. Allora i massimi comuni divisori di $a$ e $b$ sono $d$ e $-d$.

*Corollario*:
Due numeri interi non entrambi nulla hanno esattamente due massimi comuni divisori, che sono un l'opposto dell'altro.

*Notazione*:
Indicheremo con $MCD(a,b)$ (oppure $(a,b)$ quando non è ambiguo) il massimo comune divisore tra $a$ e $b$.

*Proposizione*:
Un massimo comune divisore di due numeri interi non nulli (che non siano uno il divisore dell'altro) è l'ultimo resto non nullo che compare nell'algoritmo delle divisioni successive.

*Dimostrazione*:

Dalle note.

*Definizione*:
Due numeri interi si dicono coprimi se gli unici loro divisori comuni sono $1$ e $-1$.

*Corollario*:
Siano $a,b\in \mathbb{Z}$ non entrambi nulli. Allora $a$ e $b$ sono coprimi se e solo se $(a,b)=1$.

*Dimostrazione*:
L'implicazione verso sinistra è banale. Per l'altra basta osservare che, se $1$ è un massimo comune divisore di due interi, allora ogni divisore comune divide $1$, ed è quindi uguale a $1$ o $-1\,\blacksquare$.

*Proposizione* (Corollario al Lemma di Bézout):
Siano $a,b\in \mathbb{Z}$. Allora $a$ e $b$ sono coprimi se e solo se $\exists s,t\in \mathbb{Z}$ tali che 
$$
sa+tb=1
$$
*Dimostrazione*:
Il "solo se" è il Lemma di Bézout per $d=1$. Per l'altra implicazione, detto $d$ un comune divisore di $a$ e $b$, si ha che $d$ divide $a$ e $b$, e quindi esistono $s,t\in \mathbb{Z}$ tali che $d$ divide $1$. Quindi $d\in \left\{ -1,1 \right\}\,\blacksquare$.

*Proposizione*:
Siano $a,b,c\in \mathbb{Z}$. Se $a|bc$, e $a$ e $b$ sono coprimi allora $a|c$.

*Dimostrazione*:
Esistono $s,t\in \mathbb{Z}$ tali che $sa+tb=1$. Segue che $$
c=1\cdot c=(sa+tb)c=sac+tbc.
$$
Ma per ipotesi $a$ divide questa somma, e quindi $a|c$.

*Corollario*:
Se $a,b$ sono interi non entrambi nulla, e $d=(a,b)$, allora $\frac{a}{d}$ e $\frac{b}{d}$ sono coprimi.

*Definizione*:
Siano $a,b\in \mathbb{Z}$. Allora si dice minimo comune multiplo di $a$ e $b$ ogni numero intero $h$ tale che:
1. $a|h$ e $b|h$
2. $\forall k\in \mathbb{Z}$ tale che $a|k$ e $b|k$, si ha che $h|k$.

*Osservazione*:
$mcd(a,b)=\frac{ab}{MCD(a,b)}$.

**Numeri primi. Teorema Fondamentale dell'Aritmetica**

*Definizione*:
Un numero intero $p$, diverso di $0,1$ e $0-1$ si dice primo se $\forall a,b\in \mathbb{Z}$:
$$
a|ab\implies p|a \text{ oppure } p|b
$$
Altrimenti $p$ si dice composto.

*Definizione*:
Un numero intero $p$, diverso da $0,1,-1$ si dice irriducibile se, $\forall a,b\in \mathbb{Z}$
$$
p=ab \implies a \text{ è invertibile oppure } b \text{ è invertibile}.
$$
Altrimenti $p$ si dice riducibile.

Queste due nozioni sono equivalenti come risulta dal seguente lemma:

*Lemma*:
Sia $p$ un numero intero diverso da $0,1,-1$. Allora sono fatti equivalenti:
1. $p$ è primo
2. $p$ è irriducibile
3. i divisori di $p$ sono $1,-1,p,-p$.

*Dimostrazione*:
Dimostriamo che $1)\implies 2)$. Sia $p$ primo, e siano $a,b\in \mathbb{Z}$ tali che $p=ab$. Essendo $p$ non nullo, anche $a,b$ sono non nulli. Inoltre, $p|ab$, quindi $p|a$ oppure $p|b$. Nel primo caso $a=pq$, per qualche $q\in \mathbb{Z}$, perciò si ha $a=abq$, da cui, essendo $a$ cancellabile, si deduce che $bq=1$. Quindi $b$ è invertibile. Analogamente si deduce lo stesso per $a$. ciò prova che $p$ è irriducibile.
$2)\implies3)$. Sia $p$ irriducibile, e sia $a$ un divisore di $p$. Allora si ha che $p=ab$ per quale $b\in \mathbb{Z}$. Segue che $a$ è invertibile oppure $b$ è invertibile. Nel primo caso, $a\in\left\{ 1,-1 \right\}$. Nel secondo $a\in \left\{ p,-p \right\}$. Dunque i divisore di $p$ sono $1,-1,p,-p$.
$3) \implies 1)$. Siano $a,b\in \mathbb{Z}$ tali che $p|ab$. Sia $d$ un massimo comune divisore di $a,p$. Allora $d$ è un divisore di $p$, e quindi $d\in \left\{ 1,-1 \right\}$ oppure $d\in \left\{ p,-p \right\}$. In ogni caso allora o $p|a$ oppure $p|b$, ciò prova che $p$ è primo $\blacksquare.$

*Lemma*:
Sia $p$ un primo e siano $a_{1},\dots,a_{r}\in \mathbb{Z}$ tali che $p|a_{1}\cdots a_{r}$. Allora $p|a_{i}$ per qualche $i\in \left\{ 1,\dots,r \right\}$.

*Teorema*(Teorema fondamentale dell'Aritmetica o di Fattorizzazione Unica):
Sia $n\in \mathbb{Z},\, n>1$. Allora esistono per qualche intero positivo $s$, $s$ interi positivi primi $p_{1},p_{2},\dots,p_{s}$ tali che:
$$
n=p_{1}p_{2}\cdots p_{s}.
$$
Inoltre il numero $s$ ed i numeri primi $p_{1},p_{2},\cdots p_{s}$ sono univocamente determinati.

*Dimostrazione*:
Supponiamo che per assurdo esista un numero intero maggiore di $1$ per il quale non esiste una decomposizione come quella richiesta. Allora l'insieme $X$ di tali numeri è un sottoinsieme non vuoto di $\mathbb{N}$ ed in quanto tale, per il principio del minimo, ammette minimo $m$. In particolare $m$ non è un primo, quindi è riducibile. Quindi esistono $a,b\in \mathbb{Z}$ non invertibili tali che $m=ab$. Essendo anche $m$ positivo, possiamo suppore $SPG$, che $a,b$ siano entrambi positivi. Allora essi sono entrambi maggiori di $1$. In particolare, da $a>1$ segue che $b=\frac{m}{a}<m$. Quindi $b\not\in X$, e pertanto $b$ si scrivo come prodotto di interi positivi. Ma per simmetria lo stesso è anche vero per $a$. Combinando le due si ha che anche $m$ è prodotto di interi primi positivi, contro l'ipotesi. Ciò prova che ogni intero maggiore di $1$ ammette una decomposizione in fattori primi.
Supponiamo ora che il numero intero positivo $n$ ammetta, oltre alla decomposizione di prima, anche la seguente decomposizione, dove $t$ è un intero positivo e $q_{1},\dots,q_{t}$ sono interi primi positivi:
$$
n=q_{1}\cdots q_{t}
$$
Proviamo allora che $s=t$ e che, a meno di riordinare i fattori in $1)$ e $2)$, si ha $p_{i}=q_{i}$ per ogni $i=1,\dots,s$. Procediamo per induzione su $s$. Se $s=1$, allora $n=p_{i}$ è primo. Segue quindi che $t=1$. Se fosse $t\geq 2$, avremmo che $n$ sarebbe il prodotto di $q_{1}$ e $q_{2}\cdots q_{t}$, che sono numeri naturali maggiori di $1$ e quindi non invertibili. $n$ sarebbe riducibile e dunque non primo. Quindi $n=q_{1}$, e dunque in particolare, $p_{1}=q_{1}$. Ciò prova la base dell'induzione. Supponiamo ora che $s>1$ e che la tesi sia vera per $s-1$. Segue che
$$
p_{1}\cdots p_{s}=q_{1}\cdots q_{t}.
$$
Poiché $p_{1}$ divide il prodotto al secondo membro, a meno di riordinare i fattori si ha che $p_{1}|q_{1}$. Ma essendo $q_{1}$ primo si ha che $p_{1}=\pm1$ o $p_{1}=q_{1}$, essendo $p_{1}\neq \pm 1$, segue che $p_{1}=q_{1}$. Allora, essendo $p_{1},q_{1}$ cancellabili segue che $p_{2}\cdots p_{s}=q_{1}\cdots q_{t}$. Il numero dei fattori al primo membro è $s-1$, mentre al secondo membro sono $t-1$, quindi, per ipotesi induttiva, si ah che $s-1=t-1$, cioè $s=t$, e, a meno di riordinare i fattori, per ogni $i=2,\dots,s$, $p_{i}=q_{i}\,\blacksquare$.

*Teorema*:
Esistono infiniti numeri primi.

*Dimostrazione*:
Supponiamo per assurdo che ciò non sia vero. Allora i numeri primi formano un insieme finito, diciamo $\left\{ p_{1},\dots,p_{k} \right\}$. Sia allora $N=p_{1}\cdots p_{k}+1$. Allora $N$ è un intero maggiore di uno, quindi per il teorema fondamentale dell'Aritmetica, ammette una decomposizione in fattori primi. In particolare $N$ è divisibile per un numero primo, quindi esiste un indice $i\in \left\{ 1,2,\dots,k \right\}$ tale che $p_{i}|N$. Segue però che $p_{i}|1$ che è assurdo. ciò produce la contraddizione cercata.

**La congruenza modulo $n$. Gli anelli $\mathbb{Z}_{n}$**

Sia $n$ un numero intero positivo

*Definizione*:
Siano $a,b\in \mathbb{Z}$. Diremo che $a$ è congruo a $b$ modulo $n$ se $n$ divide $a-b$. In tal caso scriveremo $a \equiv b (\text{mod }n)$.
Ciò definisce una relazione binaria su $\mathbb{Z}$ detta congruenza modulo $n$.

*Proposizione*:
La congruenza modulo $n$ è una relazione di equivalenza.

*Dimostrazione*:
$\forall a\in \mathbb{Z}$, $n$ divide $a-a= 0$, quindi $a\equiv a(\text{mod }n)$. Ciò prova che la congruenza modulo $n$ è riflessiva. Siano ora $a,b\in \mathbb{Z}$ tali che $a\equiv b(\text{mod }n)$. Allora $n$ divide $a-b$, e quindi divide anche il suo opposto $b-a$. Dunque $b\equiv a(\text{mod }n)$ che prova la simmetria.
Infine siano $a,b,c\in \mathbb{Z}$ tali che $a\equiv b(\text{mod }n)$ e $b\equiv c(\text{mod }n)$. Allora $n$ divide $a-b$ e $b-c$, quindi divide anche la loro somma ovvero $a-b+b-c=a-c$. Pertanto $a\equiv c(\text{mod }n)$, che prova la transitività della congruenza modulo $n\, \blacksquare$.

*Proposizione* (cardinalità di $\mathbb{Z}_{n}$):
Per ogni intero positivo $n$, $\mathbb{Z}_n$ ha $n$ elementi e, precisamente,
$$
\mathbb{Z}_n=\left\{ [0]_{n},\dots,[n-1]_{n} \right\}.
$$
*Dimostrazione*:
Per definizione di insieme quoziente, $\mathbb{Z}_n=\left\{ [a]_{n}|a\in \mathbb{Z} \right\}$. Poniamo $S=\left\{ [0]_{n},\dots,[n-1]_{n} \right\}$. Proviamo che $\mathbb{Z}_n=S$. Basta provare l'inclusione $\mathbb{Z}_n\subset S$. Proviamo l'altra inclusione. Sia $a\in \mathbb{Z}$. Sia $r$ il resto della divisione euclidea di $a$ per $n$. Allora, detto $q$ il quoziente della stessa divisione euclidea, si ha $a=nq+r$, e quindi $n$ divide $a-r$, cioè $a\equiv r(\text{mod }n)$. Dunque $[a]_{n}=[r]_{n}\in \mathbb{Z}$. Ciò prova che $\mathbb{Z}_n\subset S$.
Per provare che $\mathbb{Z}_n$, ha $n$ elementi, occorre provare che le classi $[0]_{n},\dots,[n-1]_{n}$, sono a due a due distinte. Ora sia $i,j\in \left\{ 0,1,\dots,n-1 \right\}$ tali che $[i]_{n}=[j_{n}]$. Poiché $i=n\cdot 0 +i$ e $0 \leq i<n$, $i$ è il resto della divisione euclidea di $i$ per $n$. D'altra parte, per ipotesi, $n$ divide $i-j$, quindi si ha che $i=nq+j$ per qualche $q\in \mathbb{Z}$. Dato che $0\leq j< n$, segue che anche $j$ è il resto della divisione di $i$ per $n$. Allora $i=j$ per l'unicità del resto $\blacksquare$.

*Proposizione*:
Siano $a,a',b,b'\in \mathbb{Z}$ tali che $a\equiv a'(\text{mod }n)$ e $b\equiv b'(\text{mod }n)$. Allora:
1. $a+b=a'+b'(\text{mod }n)$
2. $ab=a'b'(\text{mod }n)$.

*Dimostrazione*:
Per ipotesi $n$ divide $a-a'$ e anche $b-b'$. Quindi $n$ divide anche la loro somma $a-a'+b-b'=(a+b)-(a'+b')$ cioè $a+b\equiv a'+b' (\text{mod }n)$.
D'altra parte $n$ divide anche $b(a-a')$ e $a'(b-b')$ e quindi divide anche la loro somma $b(a-a')+a'(b-b')=ba-ba'+a'b'-a'b'=ab-a'b'$. Pertanto $ab\equiv a'b'(\text{mod }n)\blacksquare$.

*Proposizione*:
Sia $a\in \mathbb{Z}$. Allora $[a]_{n}\in \mathbb{Z}_n$ è invertibile se e solo se $a$ e $n$ sono coprimi.

*Dimostrazione*:
L'elemento $[a]_{n}\in \mathbb{Z}_n$ ammette un inverso $[u]_{n}\in \mathbb{Z}_n$ se e solo se esiste $u\in \mathbb{Z}$ tale che $[a]_{n}[u]_{n}=[au]_{n}=[1]_{n}$, ossia tale che $n$ divide $au-1$. Ciò equivale alla condizione: $\exists u,v\in \mathbb{Z}$ tali che $nv=au-1$, cioè tali che $au-nv=1$, che avviene se e solo se $a$ e $n$ sono coprimi.

*Proposizione*(Gli anelli $\mathbb{Z}_{p}$):
Sia $n$ un numero intero maggiore di $1$. Sono equivalenti le seguenti condizioni:
1. $n$ è primo
2. $\mathbb{Z}_n$ è un campo
3. $\mathbb{Z}_n$ è integro.

*Dimostrazione*:
$1)\implies 2)$. Sia $n$ primo. Allora $n$ non divide nessuno dei numeri $1,\dots,n-1$ e quindi, $n$ è coprimo con ciascuno di essi. Pertanto $\mathcal{U}(\mathbb{Z}_n)=\left\{ [1]_{n},\dots,[n-1]_{n} \right\}=\mathbb{Z}_n \setminus \left\{ [0]_{n} \right\}$. Ciò prova che $\mathbb{Z}_n$ è un campo.
$2) \implies 3)$ ovvio, tutti i campi sono in particolare domini di integrità.
$3) \implies 1)$ Supponiamo che $n$ non sia primo e proviamo allora $\mathbb{Z}_n$ non è integro. 