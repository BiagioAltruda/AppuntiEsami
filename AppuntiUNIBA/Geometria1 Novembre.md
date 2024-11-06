*Proposizione*:
Sia $A\in M_{m,n}(\mathbb{F})$ una matrice. sia $U$ una sua riduzione a scala, ottenuta da $A$ attraverso le operazioni elementari di riga. Allora:
1. $Row(A)=Row(U)$. (Lo spazio generato dalle righe della matrice).
2. Le righe non nulle di $U$ formano una base di $Row(U)$. In particolare $rg^{Row}(U)=rg^{Row}(A)=\#\text{ di pivot di }U$. (Il rango per righe).

*Dimostrazione*:
2. Siano $p_{1},\dots,p_{r}$ i pivot della matrice $U$ ridotta a scala. Mostriamo che le righe non nulle di $U$ sono linearmente indipendenti. Supponiamo, senza perdita di generalità, che i pivot si trovino sulle prime $r$ colonne. Cioè: $$
U=\begin{pmatrix}
p_{1} & *&*&\dots&*\\ 0&p_{2}&*&\dots&* \\
0&0&p_{3}&\dots&\dots \\ \\
0&\dots&\dots&p_{r}&* \\
0&0&0&0&0

\end{pmatrix}
$$
Siano $U_{1},\dots U_{r}$ le righe non nulle di $U$. Consideriamo una loro combinazione lineare a coefficienti in $\mathbb{F}$. Tali che $$
t_{1}U_{1}+\dots+t_{r}U_{r}=0
$$
Leggendo l'equazione di sopra componente per componente. Quindi dalla prima colonna otteniamo $t_{1}p_{1}=0$ ma $p_{1}\neq 0$ allora $t_{1}=0$. Per la seconda: $t_{1}*+t_{2}p_{2}+0+\dots+0$, essendo $t_{1}=0\implies t_{2}=2$ dato che $p_{2}\neq 0$ dato che è un pivot. Avanti così otteniamo che $\forall i=1,\dots,r,\,t_{i}=0$. Quindi le righe di $U$ sono linearmente indipendenti.
Segue che $U_{1},\dots,U_{r}$ formano una base di $Row(U)$. In particolare $\dim Row(U)=\#\text{ pivot}=r,$ per il punto $1)$, allora anche $\dim rg^{Row}(A)=r\,\blacksquare$.

*Osservazione*:
Sia $A\in M_{m,n}(\mathbb{F})$, sia $U$ una riduzione a scala di $A$ e $r=rg^{Row}(U)=rg^{Row}(A)$. Allora: 
1. $r\leq m$
2. $r\leq n$.

*Dimostrazione*:
1. Vero perché $r=\dim Row(U)\leq m$, considerando che $m$ è il numero di generatori di $Row(U)$.
2. I pivot $p_{1},\dots,p_{r}$ appartengono a colonne distinte, allora $n\geq r$ $\blacksquare$. 

*Teorema*(di Cramer per matrici quadrate):
Sia $Ax=b$ un sistema lineare sul campo $\mathbb{F}$ di $n$ equazioni in $n$ incognite. Se $rg^{Row}(A)=n$, ovvero è massimo, il sistema ammette una soluzione, ed è unica.

*Dimostrazione*:
Sia $U$ una matrice a scala ottenuta da $A$ per trasformazioni elementari di riga. Passiamo dal sistema $Ax=b$ al sistema equivalente $Ux=b'$, dove $(U|b')$ si ottiene da $(A|b)$ con lo stesso procedimento. Poiché, per ipotesi, $rg^{Row}(A)=rg^{Row}(U)=n$, ho esattamente $n$ pivot, $p_{1},\dots,p_{n}$. Con $p_{1}$ sulla prima colonna $(j(1)=1)$, e così via fino a $p_{n}$ sulla $n$-esima colonna $(j(n)=n)$. Allora $U$ è una matrice triangolare superiore, con i pivot sulla diagonale principale, in particolare ci sono tutti elementi non nulli. Risolviamo il sistema equivalente $Ux=b'$. Quindi $$
\begin{cases}
p_{n}x_{n}=b_{n}' \\
p_{n-1}x_{n-1}+u_{n}x_{n} \\
\dots \\
\dots \\
p_{1}x_{1}+u_{2}x_{2}+\dots+u_{n}x_{n}
\end{cases}
$$
Ricaviamo che $x_{n}=\frac{b'_{n}}{p_{n}}$ dato che $p_{n}\neq 0$.
$$
\begin{cases}
x_{n}=\frac{b'_{n}}{p_{n}} \\
p_{n-1}x_{n-1}+u_{n-1}\frac{b'_{n}}{p_{n}}=b'_{n-1} \\
\dots \\
\dots \\
\dots
\end{cases}
$$
Ricavando univocamente, per sostituzioni successive, gli $x_{i}$, con $i=1,\dots,n\,\blacksquare$.

*Esempio*:
Sistema a $3$ equazioni in $3$ incognite:
$$
\begin{cases}
x_{1}+x_{3}=2 \\
2x_{1}-6x_{2}+4x_{3}=5 \\
x_{1}-3x_{2}+5x_{3}=1
\end{cases}
$$
Di matrice completa: $$
(A|b)=\begin{pmatrix}
1&0&1&2 \\
2&-6&4&5 \\
1&-3&5&1
\end{pmatrix}
$$
Col metodo di Gauss: $$
\begin{pmatrix}
1&0&1&2 \\
2&-6&4&5 \\
1&-3&5&1
\end{pmatrix} \to R_{2}-2R_{1}\to \begin{pmatrix}
1&0&1&2 \\
0&-6&2&1 \\
-1&-3&5&1
\end{pmatrix}\to R_{3}-R_{1}\to  \begin{pmatrix}
1&0&1&2 \\
0&-6&2&1 \\
0&-3&4&1
\end{pmatrix}\to
$$
$$
 \to R_{3}-\frac{1}{2}R_{2}\to   \begin{pmatrix}
1&0&-1&2 \\
0&-6&2&1 \\
0&0&3&-\frac{3}{2}
\end{pmatrix}=(U|b').
$$
Segue che: $$
\begin{cases}
3x_{3}=-\frac{3}{2}\implies x_{3}=-\frac{1}{2} \\ 
x_{2}=-\frac{1}{3} \\
x_{1}=\frac{5}{2}.
\end{cases}
$$
Quindi $Sol(Ax=b)=\left\{ \begin{pmatrix} \frac{5}{2}\\ \frac{-1}{3}\\ \frac{-1}{2}\end{pmatrix} \right\}$.

*Proposizione*(Formula di Cramer per sistemi $2\times 2$):
Sia $A=\begin{pmatrix}a&b\\c&d\end{pmatrix}\in M_{2,2}(\mathbb{F})$. Consideriamo il sistema $$
A\begin{pmatrix}
x\\y
\end{pmatrix}=\begin{pmatrix}
e\\f
\end{pmatrix}
$$

Se $ad-cb\neq 0$ allora, $rg^{Row}(A)=2$, e quindi il sistema ammette una soluzione unica: $$
\begin{pmatrix}
x\\ y
\end{pmatrix}=\begin{pmatrix}
\frac{ed-bf}{ad-cb} \\ \frac{af-ce}{ad-cb}
\end{pmatrix}.
$$

*Dimostrazione*:
Considero la matrice completa: $$
\begin{pmatrix}
a&b&e\\ c&d&f
\end{pmatrix}
$$ e la riduco a scala.
Supponiamo $a\neq 0$. Tramite l'operazione $R_{2}=R_{2}- \frac{cR_{1}}{a}$, quindi: $$
\begin{pmatrix}
a&b&e \\
0& d-\frac{cb}{a}&f-\frac{ec}{a}
\end{pmatrix}
$$
dalla seconda riga ricaviamo $y$: $y\left( d- \frac{cb}{a} \right)=f- \frac{ec}{a}$.
Se $a=0$, allora $c\neq 0$, altrimenti la matrice non avrebbe rango massimo. Procedo nello stesso modo scambiando però la prima e la seconda riga $\blacksquare$.

*Teorema*(Rouché-Capelli, struttura delle soluzioni di un sistema lineare generale):
Sia dato un sistema lineare $Ax=b$ in $m$ equazioni ed $n$ incognite. Allora: 
1. Il sistema ha soluzione se e solo se $rg^{Row}(A)=rg^{Row}(A|b)$.
2. Se il sistema ha soluzione, sia $r=rg^{Row}(A)=rg^{Row}(A|b)$, allora $Sol(Ax=b)$ dipende da $n-r$ parametri. Ovvero esistono $v_{0},v_{1},\dots,v_{n-r}$ vettori di $\mathbb{F}^{n}$, tali che $Sol(Ax=b)=\left\{ v=v_{0}+t_{1}v_{1}+t_{2}v_{2}+\dots+t_{n-r}v_{n-r}|\, t_{1},\dots,t_{n-r}\in \mathbb{F} \right\}$.
3. $Sol(Ax=0)=Ker(A)=\left\{ v=t_{1}v_{1}+t_{2}v_{2}+\dots+t_{n-r}v_{n-r}|\,t_{1},\dots,t_{n-r}\in \mathbb{F} \right\}$.

*Dimostrazione*:
Riduco a scala la matrice completa $(A|b)$ e ottengo $(U|b')$. $$
(U|b')=\begin{pmatrix}
0&\dots&0&p_{1}&*&\dots&*&b_{1}' \\
0&\dots&0&0&\dots&p_{2}&*&b_{2}' \\
\dots &\dots&\dots&\dots&\dots&\dots&\dots&\dots\\
\dots&\dots&\dots&\dots&\dots&\dots&p_{r}&b_{r}' \\
0&0&0&0&0&0&0&b_{r+1} \\
\dots &\dots&\dots&\dots&\dots&\dots&\dots&\dots\\

\end{pmatrix}
$$
Siano quindi $p_{1},\dots,p_{r}$ i pivot di $A$. Ci sono $2$ casi:
$i)$ $r<m$ cioè ci sono righe nulle in $U$, ed esista $b_{k}'\neq 0,\,m\geq k\geq r+1$. La $k-$esima equazione è impossibile, dato che avremmo $0=b_{k}'\neq 0$, il sistema non ha soluzione. Segue anche che $rg^{Row}(U)=r$, mentre $rg^{Row}(U|b')>r$, dato che $b'_{k}$ diventa un pivot in più rispetto a quelli di $U$.
$ii)$ $r=m \,\vee (r<m\,\wedge\,b'_{k}=0,\,\forall k= r+1,\dots,m)$, il caso complementare a $i)$. Ovvero il caso dove $rg^{Row}(U)=rg^{Row}(U|b')$. Mostriamo che in questo caso il sistema ha soluzioni, dipendenti da $n-r$ parametri.
Chiamiamo variabili dipendenti le $r$ variabili del sistema corrispondenti ai pivot. Mentre chiamiamo variabili libere le $n-r$ rimanenti variabili.
Risolvo il sistema per sostituzione all'indietro partendo dall'ultima riga. $$
(U|b')=\begin{pmatrix}
0&\dots&0&p_{1}&*&\dots&*&b_{1}' \\
0&\dots&0&0&\dots&p_{2}&*&b_{2}' \\
\dots &\dots&\dots&\dots&\dots&\dots&\dots&\dots\\
\dots&\dots&\dots&\dots&\dots&\dots&p_{r}&b_{r}' \\
0&0&0&0&0&0&0&0 \\
\dots &\dots&\dots&\dots&\dots&\dots&\dots&\dots\\

\end{pmatrix}
$$
Ottenendo dall'ultima riga non nulla: $$
p_{r}x_{k}+c_{k+1}x_{k+1}+\dots+c_{n}x_{n}=b_{r}' \,\,(*)
$$
Osservo che $x_{k}$ è l'ultima variabile dipendente. Le variabili $x_{k+1},\dots,x_{n}$ sono libere. Da quest'equazione $(*)$ ricavo $x_{k}$ in funzione di variabili libere, dato che il coefficiente di $x_{k}$, $p_{r}$, è non nullo. Segue che $$
x_{k}=\frac{b_{r}'}{p_{r}}-\frac{c_{k+1}x_{k+1}}{p_{r}}-\dots-\frac{c_{n}x_{n}}{p_{r}}. (**)
$$
Sostituiamo $x_{k}$ nella penultima equazione: $$
p_{r-1}x_{h}+*x_{h+1}+\dots+*x_{n}=b'_{r-1}.
$$
dove $h$ è la colonna corrispondente al pivot $p_{r-1}$.
Le variabili che compaiono sono tutte libere tranne $x_{k}$, che abbiamo già ricavato, e quindi sostituiamo il valore già trovato $(**)$.
Ricavo anche $x_{h}$ in funzione delle variabili libere. Procedo in questo modo fino ad arrivare alla prima riga. Ottenendo tutte le variabili dipendenti in funzione da quelle libere e dai termini noti.
Chiamiamo $t_{1},..,t_{n-r}$ le $n-r$ variabili libere, ottengo ciascuna delle variabili dipendenti nella forma: $$
x_{i}=d_{i}+a_{i,1}t_{1}+a_{i,2}t_{2}+\dots+a_{i,n-r}t_{n-r},\quad d_{i},a_{i,j}\in \mathbb{F},\, i\in I=\left\{ 1,\dots,n \right\} ,\,|I|=r.
$$
Ordinando le soluzioni, sia $v_{0}=(x_{i})_{i\in I}$ soluzione ottenuta dando a $t_{1},\dots,t_{n-r}$ il valore $0$. $v_{1}=$ il vettore formato dai coefficienti di $t_{1}$, e così via.
Quindi $Sol(U|b')=\left\{ v_{0}+t_{1}v_{1}+\dots+t_{n-r}v_{n-r} \right\}\,\blacksquare$.

Ci sono $3$ casi:
1. Se $r=r'=n$ allora la soluzione esiste ed è unica.
2. Se $n>r=r'$ allora il sistema ha soluzioni dipendenti da $n-r$ parametri e si dice sottodeterminato.
3. $r\neq r'$ allora il sistema non ha soluzione.

*Teorema*(Nullità $+$ rango per matrici):
Se $A\in M_{m,n}(\mathbb{F})$ di rango $rg^{Row}(A)=r$. Allora $\dim(Ker(A))=n-r$.

*Dimostrazione*:
Se $n=r$, allora il sistema $Ax=0$ ha almeno una soluzione, quella nulla. In particolare $A$ e la sua matrice completa hanno lo stesso rango, quindi per il teorema di Rouché-Capelli la soluzione è unica: $\underline{x}=\underline{0}$.
Se, invece, $n>r$. Sempre per il teorema di Rouché-Capelli esistono $v_{1},\dots,v_{n-r}$ vettori tali che $Sol(Ax=0)=Ker(A)=\left\{ t_{1}v_{1}+\dots+t_{n-r}v_{n-r}|\, t_{i}\in \mathbb{F},\, i=1,\dots,n-r \right\}$. Quindi $\dim Ker(A)=n-r$, dato che i $v\in Ker(A)$ si scrivono in modo univoco come combinazione $v_{1},\dots,v_{n-r}$, loro formano una base, di $n-r$ elementi $\blacksquare$.

*Osservazione*:
Stiamo dicendo che $\dim Ker(A)+rg^{Row}(A)=n$.


----------

**Spazio delle applicazioni lineari e spazio duale**

Siano $S,T:V\to W$ applicazioni lineare definite su $V$ e $W$ spazi vettoriali sul campo $\mathbb{F}$. Sia $\lambda \in \mathbb{F}$. 

*Definizione*:
$$
S+T:V\to W,\,\lambda S:V\to W
$$
dove:
$$
(S+T)(v)=S(v)+T(v),
$$
$$
\lambda S(v)=\lambda S(v).
$$
*Osservazione*:
Se $S,T$ sono applicazioni lineari, allora $S+T$ e $\lambda S$ sono applicazioni lineari.

*Dimostrazione*:
Dimostriamo che $S+T$ è lineare. Siano $v_{1},v_{2}\in V$ e $\alpha_{1},\alpha_{2}\in \mathbb{F}$. Allora: $$
(S+T)(\alpha_{1}v_{1}+\alpha_{2}v_{2})=S(\alpha_{1}v_{1}+\alpha_{2}v_{2})+T(\alpha_{1}v_{1}+\alpha_{2}v_{2}) =
$$
$$
=\alpha_{1}S(v_{1})+\alpha_{2}S(v_{2})+\alpha_{1}T(v_{1})+\alpha_{2}T(v_{2})=
$$
$$
=\alpha_{1}(S(v_{1})+T(v_{1}))+\alpha_{2}(S(v_{2})+T(v_{2}))=\alpha_{1}(S+T)(v_{1})+\alpha_{2}(S+T)(v_{2})\,\blacksquare.
$$

*Osservazione*:
Si può mostrare che la somma e il prodotto per scalare appena introdotti verificano gli assiomi di spazio vettoriale.

*Definizione*:
L'insieme $\mathcal{L}(V,W)$ delle applicazioni lineari da $V$ in $W$ munito delle operazioni di somma e prodotto per scalare è uno spazio vettoriale.
Lo spazio $\mathcal{L}(V,\mathbb{F})$ viene detto spazio duale di $V$. Denoteremo il duale di $V$ con $V'$, $V^{*}$,$V^{V}$.

*Definizione*:
Sia $V$ spazio vettoriale sul campo $\mathbb{F}$, e sia $V^{*}$ il suo spazio duale. Sia $\mathcal{B}=\left( v_{1},\dots,v_{n} \right)$ una base di $V$. Definiamo la base duale $\mathcal{B}^{*}$ di $\mathcal{B}$, quella tale che: $\mathcal{B}^{*}=(f_{1},\dots,f_{n})$, dove $f_{i}:V\to \mathbb{F}$ tale che:
$$f_{i}(v_{j})=\delta_{i,j}=\begin{cases}
0&\text{ se } i\neq j \\
1&\text{ se }i=j
\end{cases}$$
$\delta_{i,j}$ si dice delta (o simbolo) di Kronecker.
Ad esempio $f_{1}(v_{1})=1$ e $f_{1}(v_{2})=f_{1}(v_{2})=\dots=f_{1}(v_{n})=0$.

*Esempio*:
Sia $V=\mathbb{R}^{3}$, sia $\mathcal{B}=\left( e_{1},e_{2},e_{3} \right)$, la base canonica.
$(\mathbb{R}^{3})^{*}=\left\{ f:\mathbb{R}^{3}\to \mathbb{R}|\,f \text{ è lineare} \right\}$. Ad esempio $g:\mathbb{R}^{3}\to \mathbb{R}$, $g\begin{pmatrix}x_{1}\\x_{2}\\x_{3}\end{pmatrix}=3x_{1}-2x_{2}-x_{3}$, oppure $h:\mathbb{R}^{3}\to \mathbb{R}$, $h\begin{pmatrix}x_{1}\\x_{2}\\x_{3}\end{pmatrix}=-x_{1}+x_{3}$.
Cerchiamo $\mathcal{B}^{*}=\left( f_{1},f_{2},f_{3} \right)$ base duale di $\mathcal{B}$.
$f_{1}:\mathbb{R}^{3}\to \mathbb{R}$ è un'applicazione lineare tale che $f_{1}(e_{1})=1$ e $f_{1}(e_{2})=f_{1}(e_{3})=0$.
$f_{1}\begin{pmatrix}x_{1}\\x_{2}\\x_{3}\end{pmatrix}=\alpha_{1}x_{1}+\alpha_{2}x_{2}+\alpha_{3}x_{3}$.
Deve valere che $f_{1}\begin{pmatrix}1\\0\\0\end{pmatrix}=\alpha_{1}=1$. $f_{1}\begin{pmatrix}0\\1\\0\end{pmatrix}=\alpha_{2}=0$. $f_{1}\begin{pmatrix}0\\0\\1\end{pmatrix}=\alpha_{3}=0$.
Quindi $f_{1}:\mathbb{R}^{3}\to \mathbb{R}$ è la funzione $f_{1}\begin{pmatrix}x_{1}\\x_{2}\\x_{3}\end{pmatrix}=x_{1}$. Con gli stessi conti $f_{2}\begin{pmatrix}x_{1}\\x_{2}\\x_{3}\end{pmatrix}=x_{2}$ e $f_{3}\begin{pmatrix}x_{1}\\x_{2}\\x_{3}\end{pmatrix}=x_{3}$.

Sempre in $\mathbb{R}^{3}$, sia $\mathcal{C}=\left( v_{1}=\begin{pmatrix}1\\2\\0\end{pmatrix},v_{2}=\begin{pmatrix}0\\0\\3\end{pmatrix},v_{3}=\begin{pmatrix}1\\1\\1\end{pmatrix} \right)$. Cerchiamo $\mathcal{C}^{*}=\left( g_{1},g_{2},g_{3} \right)$, $g_{i}:\mathbb{R}^{3}\to \mathbb{R}$ tali che $g_{i}(v_{j})=\delta_{i,j}$.
Sappiamo che $\forall v=\begin{pmatrix}x_{1}\\x_{2}\\x_{3}\end{pmatrix}\in V,\,\exists!\gamma_{1},\gamma_{2},\gamma_{3}\in \mathbb{R}$ tali che $v=\gamma_{1}v_{1}+\gamma_{2}v_{2}+\gamma_{3}v_{3}$.
Quindi $g_{1}\begin{pmatrix}x_{1}\\x_{2}\\x_{3}\end{pmatrix}=\gamma_{1},\,g_{2}\begin{pmatrix}x_{1}\\x_{2}\\x_{3}\end{pmatrix}=\gamma_{2},\,g_{3}\begin{pmatrix}x_{1}\\x_{2}\\x_{3}\end{pmatrix}=\gamma_{3}$.
Calcoliamo $\gamma_{1},\gamma_{2},\gamma_{3}$.
$$
\begin{cases}
x_{1}=\gamma_{1} +\gamma_{3}\\
x_{2}=2\gamma_{1}+\gamma_{3}\\
x_{3}=3\gamma_{2}+\gamma_{3}
\end{cases}=
\begin{cases}
\gamma_{1}=x_{1}-\gamma_{3} \implies \gamma_{1}=-x_{1}+x_{2} \\
x_{2}=2\gamma_{1}-2x_{1}-2\gamma_{3}+\gamma_{3} \implies \gamma_{3}=2x_{1}-x_{2} \\
\gamma_{2}=\frac{1}{3}(-2x_{1}+x_{2}+x_{3}).
\end{cases}
$$
Allora, $g_{1}\begin{pmatrix}x_{1}\\x_{2}\\x_{3}\end{pmatrix}=-x_{1}+x_{2}$. $g_{1}(v_{1})=1$, $g_{1}(v_{2})=0$, $g_{1}(v_{3})=0$.
$g_{2}\begin{pmatrix}x_{1}\\x_{2}\\x_{3}\end{pmatrix}=-\frac{2}{3}x_{1}+\frac{1}{3}x_{2}+\frac{1}{3}x_{3}$ e $g_{3}\begin{pmatrix}x_{1}\\x_{2}\\x_{3}\end{pmatrix}=2x_{1}-x_{2}$.

*Esercizio*:
In $\mathbb{R}_{3}[x]$ calcolare la base duale di $\mathcal{B}=\left( 2t-1,3t^{2}+2,t^{3}+t,t^{2} \right)$.

------
Ricordiamo che se $f:A\to B$ e $g:C\to D$ funzioni. Se $B\subset C$ possiamo definire la composizione $g\circ f:A\to D$. Definita come $(g\circ f)(a)=g(f(a))$.

*Proposizione*:
Se $S:U\to V$ e $T:V\to W$ sono applicazioni lineari tra gli spazi vettoriali $U,V,W$ sul campo $\mathbb{F}$. Allora la composizione $T\circ S:U\to W$ è lineare.

*Dimostrazione*:
Siano $u_{1},u_{2}\in U,\,\alpha_{1},\alpha_{2}\in \mathbb{F}$. Allora $(T\circ S)(\alpha_{1}u_{1}+\alpha_{2}u_{2})=$ $$
=T(S(\alpha_{1}u_{1}+\alpha_{2}u_{2}))=T(\alpha_{1}S(u_{1})+\alpha_{2}S(u_{2}))=\alpha_{1}T(S(u_{1}))+\alpha_{2}T(S(u_{2})).
$$
Allora: $$
=\alpha_{1}(T\circ S)(u_{1}) + \alpha_{2}(T\circ S)(u_{2})\,\blacksquare.
$$
*Osservazione*:
Ogni volta che sono ben definite, valgono le seguenti uguaglianze:
1. $((S_{1}+S_{2}))\circ T=S_{1}\circ T +S_{2}\circ T$
2. $(S\circ (T_{1}+T_{2}))=(S\circ T_{1})+(S\circ T_{2})$
3. $((\lambda S)\circ T)=\lambda(S\circ T)= (S\circ (\lambda T))$.

*Esempio*:
$S:\mathbb{R}^{2}\to \mathbb{R}^{4}$, $T:\mathbb{R}^{4}\to \mathbb{R}^{3}$. Con $S\begin{pmatrix}x_{1}\\x_{2}\end{pmatrix}=\begin{pmatrix}-x_{1}+x_{2}\\2x_{1}\\x_{1}-3x_{2}\\x_{2}\end{pmatrix}$, e $T\begin{pmatrix}y_{1}\\y_{2}\\y_{3}\\y_{4}\end{pmatrix}=\begin{pmatrix}y_{1}-y_{2}\\y_{1}+y_{3}\\y_{1}+y_{2}+y_{3}\end{pmatrix}$.
Si può definire $(T\circ S)$ ma non $(S\circ T)$. 
Quindi $(T\circ S)\begin{pmatrix}x_{1}\\x_{2}\end{pmatrix}=T\left( S\begin{pmatrix}x_{1}\\x_{2}\end{pmatrix} \right)=T\begin{pmatrix}-x_{1}+x_{2}\\2x_{1}\\x_{1}-3x_{2}\\x_{2}\end{pmatrix}=\begin{pmatrix}-x_{1}+x_{2}-2x_{1}\\-x_{1}+x_{2}-3x_{2}\\-x_{1}+x_{2}+2x_{1}+x_{1}-3x_{2}\end{pmatrix}=\begin{pmatrix}-3x_{1}+x_{2}\\-2x_{2}\\2x_{1}-x_{2}\end{pmatrix}$.

Se $S:V\to W$ e $T:W\to V$ posso definire sia $(S\circ T)$ che $(T\circ S)$.

Vale che per ogni spazio vettoriale $V$, abbiamo definito $id_{V}:V\to V$ tale che $\forall v\in V,\,id_{V}(v)=v$.
In particolare $S(id_{V}(v))=S(v)=id_{W}(S(v))=S(v)$.
Cioè l'applicazione identica è l'elemento neutro della composizione tra applicazioni lineari.

Ci chiediamo quando $(S\circ T)$ è l'inversa di $(T\circ S)$.

*Definizione*:
Diremo che un'applicazione lineare $T:V\to W$ è invertibile se $\exists S:W\to V$, applicazione lineare, tale che $(T\circ S)=id_{W}$ e $(S\circ T)=id_{V}$.

*Osservazione*:
La composizione di funzioni è associativa.

*Proposizione*:
Se $T:V\to W$ è invertibile, allora ammette un'unica inversa. Che denoteremo con $T^{-1}$.


*Dimostrazione*:
Siano $S_{1},S_{2}:W\to V$ inverse di $T$. Allora: $$
(T\circ S_{1})=(T\circ S_{2})=id_{W}
$$
e anche $$
(S_{1}\circ T)=(S_{2}\circ T)=id_{V}.
$$
Dimostriamo che $S_{1}=S_{2}$. $$
S_{1}=(S_{1}\circ id_{W})=(S_{1}\circ (T\circ S_{2}))=((S_{1}\circ T)\circ S_{2})= (id_{V}\circ S_{2})=S_{2}\,\blacksquare.
$$
*Proposizione*:
Sia $T:V\to W$ lineare. T è invertibile se e solo se $T$ è bigettiva.

*Dimostrazione*:
$T$ è bigettiva se e solo se $\exists S:W\to V$ tale che $(S\circ T)=id_{V}$.
Dimostriamo che $S$ è lineare. Siano $w_{1},w_{2}\in W$ e siano $\beta_{1},\beta_{2}\in \mathbb{F}$. Allora valutiamo $$
S(\beta_{1}w_{1}+\beta_{2}w_{2}).
$$
Essendo $T$ bigettiva, è anche suriettiva, quindi $\exists v_{1},v_{2}\in V$ tali che $T(v_{1})=w_{1}$ e $T(v_{2})=w_{2}$. Allora $$
S(\beta_{1}T(v_{1})+\beta_{2}T(v_{2}))=S(T(\beta_{1}v_{1}+\beta_{2}v_{2}))=$$$$=(S\circ T)(\beta_{1}v_{1}+\beta_{2}v_{2})=\beta_{1}v_{1}+\beta_{2}v_{2}=\beta_{1}S(w_{1})+\beta_{2}S(w_{2})\,\blacksquare.
$$
*Corollario*:
Sia $T:V\to W$ lineare con $\dim V=\dim W$. Allora sono fatti equivalenti: 
1. $T$ è invertibile
2. $T$ è iniettiva
3. $T$ è suriettiva.

*Definizione*:
Siano $V$ e $W$ spazi vettoriali tali che $\exists\, T:V\to W$ lineare e invertibile. Allora $V$ e $W$ si dicono isomorfi e $T$ si dice isomorfismo.