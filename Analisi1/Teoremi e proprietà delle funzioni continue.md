*Proposizione 6.19*:
se $f$ è continua in $x_{*}$ e se esiste un intorno $V_{0}\in \mathcal{F_{x_{*}}}$ tale che:
1. $x_{*}\in \text{dom}g$,
2. $g(x)=f(x) \text{ in dom}g\cap V_{0}$,
Allora $g$ è continua in $x_{*}$

Ad esempio la funzione $$
g(x)=
\begin{cases}
1+\sin x\quad \text{se }x\geq0 \\ \cos x\qquad\,\,\,\, \text{se }x<0
\end{cases}
$$
è continua, infatti, se $x_{*}>0$ la funzione $g$ coincide nell'intorno $(0,2x_{*})$ di $x_{*}$ con la funzione continua $1+\sin x$, dunque $g$ è continua in $x_{*}$. si può fare lo stesso ragionamento per $x<0$.

---
*Teorema 6.20* (limitatezza locale):
Se $f$ è continua in $x_{*}$, esiste un intorno $V_{0}\in \mathcal{F_{x_{*}}}$ tale che $f_{\Big|V_{0}}$ è limitata.

---
*Teorema 6.21* (Permanenza del segno):
se $f$ è continua in $x_{*}$ ed $f(x_{*})\neq0$, esiste un intorno $V_{0}\in \mathcal{F_{x_{*}}}$tale che $f_{\Big|V_{0}}$ ha segno costante.

---
*Teorema 6.22*:
se $f$ è continua in $x_{*}$ e $g$ è continua in $f(x_{*})$ allora $g\circ f$ è continua in $x_{*}$.

---
*Teorema 6.23*: Somma, prodotto, inverse, valore assoluto, massimo e minimo di funzioni continue sono continue (se la funzione è ben definita).

---
*Proposizione 6.25*:
Sia $A\subset \mathbb{R}$ un insieme limitato superiormente (inferiormente), sia $f$ una funzione continua tale che $A \cup \left\{ \sup A \right\}\subset \text{dom}f \quad(A \cup \left\{ \inf A \right\}\subset \text{dom}f)$, se $f$ è debolmente crescente si ha:
$$
\sup_{A}f=f(\sup A)\qquad \left(\inf_{A}f=f(\inf A)\right),
$$
mentre se $f$ è debolmente decrescente si ha $$
\inf_{A}f=f(\sup A)\qquad \left(\sup_{A}f=f(\inf A)\right).
$$
*Dimostrazione*:
Mostriamo la prima disuguaglianza: $\forall x\leq \text{sup}_{A}\text{ è }f(x)\leq(\text{sup}A)$, e ci basta provare la disuguaglianza opposta. Presa una successione $\{a_n\}_n\subset A$ tale che $a_{n}\to \text{sup}A$, abbiamo per ogni $n$ $$
f(a_{n})\leq \sup_{A}f, 
$$
ma $f(a_{n})\to f(\sup A)$ per la continuità di $f$, così $f(\sup A)\leq\sup_{A}f.$ $\blacksquare$

---
*Proposizione 6.26*:
Se $f\in C^{0}([a,b])$ e $f(a)$ ha segno diverso da $f(b)$ allora esiste un punto $\xi \in[a,b]$ tale che $f(\xi)=0$.
*Dimostrazione*:
Osserviamo che dalle ipotesi sul segno di $f$ segue $$
f(a)f(b)\leq0
$$
Poniamo $a_{0}$=a, $b_{0}=b$ e $m_{0}=\frac{a_{0}+b_{0}}{2}$; dato che $[f(m_{0})]^{2}\geq 0$, anche $$
[f(a_{0})f(m_{0})]\,[f(m_{0})f(b_{0})]\leq 0
$$
Allora uno dei due fattori è non positivo: se fosse il primo poniamo $a_{1}=m_{0}\text{ e }b_{1}=b_{0}$. In ogni caso abbiamo
$$
\begin{cases}
a_{0}\leq a_{1}<b_{1}\leq b_{0}\\
b_{1}-a_{1}=\frac{b-a}{2^{1}} \\
f(a_{0})f(b_{0})\leq 0, & f(a_{1})f(b_{1})\leq 0
\end{cases}
$$
e poniamo $m_{1}=\frac{a_{1}+b_{1}}{2}$. Si conclude per induzione, ottenendo due successioni monotone, una crescente e una decrescente che tendono allo stesso limite $\xi$, e tali che per ogni $n$ $$
f(a_{n})f(b_{n}) \leq 0
$$
Dato che $a\leq a_{n}\leq b$, passando al limite abbiamo anche $\xi \in[a,b]$, dunque $f$ è continua nel punto $\xi$. Poiché $a_{n}\to \xi$ e $b_{n}\to \xi$, passando al limite otteniamo per la continuità di $f$
$$
[f(\xi)]^{2}\leq 0
$$
cioè $f(\xi)=0$. $\blacksquare$

---
*Teorema 6,27* (degli zeri):
se $f\in C^{0}(I)$ assume valori di segno diverso, si annulla almeno una volta in $I$.
*Dimostrazione*:
per ipotesi esistono due punti $a<b\in I$ in cui $f$ assume valori di segno diverso;. Chiaramente $[a,b]\in I$. Allora la restrizione di $f$ ad $[a,b]$ è continui in ogni punto di $[a,b]$ e soddisfa le ipotesi della proposizione precedente, dunque esiste un punto $\xi \in[a,b]$ tale che $f_{|_{[a,b]}}(\xi)=0=f(\xi)$. $\blacksquare$ ^5c6863

---
*Proposizione 6.28*:
se $f\in C^0([a,b])$ e $f(a)\leq k\leq f(b)$, esiste un punto $\xi \in[a,b]$ tale che $f(\xi)=k$.

---
*Teorema 6.29* (dei valori intermedi):
se $f\in C^0(I)$ la sua immagine è un intervallo.
*Dimostrazione*:
Deve valere che comunque scelgo $\alpha,\beta \in f(I)$ e $k\in[\alpha,\beta]$, $k\in f(I)$. Scegliamo dunque $a,b \in I$ tali che $\alpha=f(a),\,\beta=f(b)$: dobbiamo provare che $k\in f(I)$. Supponiamo $a\leq b$ e che $\alpha\leq k\leq\beta$. Allora la tesi segue applicando il teorema precedente alla restrizione di $f$ all'intervallo $[a,b]$, che è tutto contenuto in $I$. $\blacksquare$

---
*Teorema 6.32*:
Sia $f\in C^{0}(I)$, allora $f$ è iniettiva se e solo se è strettamente monotona.
*Dimostrazione*:
Sappiamo già che se $f$ è strettamente monotona allora è iniettiva. Dimostriamo per assurdo l'altra implicazione: negare che $f$ è strettamente crescente significa:
$$
\begin{cases}
\exists x_{0},y_{0}\in I: x_{0}<y_{0}\text{ e } f(x_{0})\geq f(y_{_{0}}) \\
\exists x_{1},y_{1}\in I: x_{1}<_{1}\text{ e } f(x_{1})\leq f(y_{1})
\end{cases}
$$
Dunque la differenza fra il valore di $f$ tra l'estremo destro e sinistro dell'intervallo $[x_{0},y_{0}]$ è minore o uguale a $0$. Definiamo due funzioni su $[0,1]$:
$$
x(t)=x_{0}+t(x_{1}-x_{0}),\qquad y(t)=y_{0}+t(y_{1}-y_{0})
$$
Queste sono chiaramente continue, osserviamo anche che $\forall t\in[0,1]\,\,x(t)<y(t)$ in quanto:
$$
y(t)-x(t)=(1-t)(y_{0}-x_{0})+t(y_{1}-x_{1})\qquad \forall t\in[0,1]
$$
Quindi la funzione $$
F(t)=f(y(t))-f(x(t))
$$ è definita su $[0,1]$, ed è continua perché composizione di funzioni continue, per l'ipotesi fatta vale anche
$$
F(0)=f(y_{0})-f(x_{0})\geq0,\quad F(1)=f(y_{1})-f(x_{1})\leq0
$$
Possiamo applicare il teorema degli zeri e trovare un punto in cui $F$ si annulla, $\bar{t}$, ma allora avremmo, per la definizione di $F$:
$$
f(y(\bar{t}))=f(x(\bar{t}))
$$
che implica $f$ non iniettiva. $\blacksquare$

---
*Proposizione 6.33*: Se $g$ è una funzione reale monotona definita su un intervallo $J$, allora $g$ è continua se e solo se la sua immagine $g(J)$ è un intervallo.
*Dimostrazione*: (Da scrivere)

---
*Teorema 6.34*:
se $f$ è una funzione continua e invertibile definita su un intervallo $I$, la sua inversa è continua.
*Dimostrazione*:
Segue dalle proposizioni precedenti: se $f$ è strettamente monotona, anche la sua inversa lo sarà, l'inversa è anche definita su un intervallo ed è surgettiva nell'intervallo di partenza, cioè la sua immagine è un intervallo, pertanto è continua.

---
*Teorema 6.35* (Di Weierstrass):
se $f\in C^0([a,b])$ allora ammette massimo e minimo.
*Dimostrazione*:
Dimostriamo che $f$ ha massimo, il minimo si fa applicando il risultato a  $-f$. Sia $M=\sup f,\, M\in(-\infty,+\infty)$; se $M\in \mathbb{R}$, poniamo $y_{n}=M-\frac{1}{n}$ per ogni $n\in \mathbb{N}^{+}$, altrimenti poniamo $y_{n}=n$. In ogni caso la successione $\{y_n\}_n$ è una successione che cresce ad $M$. dato che $y_{n}<M=\sup f$, per definizione di estremo superiore esiste qualche valore di $f$ maggiore di $y_{n}$, lo chiamiamo $f(x_{n})$. Vale quindi per ogni $n$:
$$
y_{n}<f(x_{n})\leq M,\qquad a\leq x_{n}\leq b
$$
per il teorema dei carabinieri, essendo $M=\lim_{ n \to \infty }y_{n}$ vale $$
f(x_{n})\to M
$$
Applicando alla successione limitata $\{x_n\}_n$ il teorema di [[Successioni#^6c5a88|Bolzano-Weierstrass]] ne possiamo estrarre una sottosuccessione convergente, $x_{n_{k}}\to x_{*}$; dato che $a\leq x_{n_{k}}\leq b$ per ogni $n$, anche $x_{*}\in[a,b]$. Allora per la continuità di $f$ otteniamo che $f(x_{n_{k}})\to f(x_{*})$ ma $\left\{ f(x_{n_{k}}) \right\}_{n}$ è una estratta di $\left\{ f(x_{n}) \right\}_{n}$, quindi per $f(x_{n_{k}})\to M$ e per l'unicità del limite abbiamo trovato un punto $x_{*}$ in cui $$
f(x_{*}) =M=\sup f
$$
Cioè l'estremo superiore è un massimo. $\blacksquare$

---
*Teorema 6.36*:
se $f\in C^{0}([a,b])$ allora $f$ è limitata.

---
*Proposizione 6.37*:
se $f\in C^{0}([a,b])$ allora l'immagine di $f$ è l'intervallo chiuso $[\min f, \max f]$

---
*Proposizione 6.38*:
Se $I$ è un intervallo e $f\in C^{0}(I)$ ha lo stesso limite ai due estremi dell'intervallo, allora $f$ ha massimo oppure minimo.

[[Funzioni lipschitziane e uniformemente continue]]
#continuità
