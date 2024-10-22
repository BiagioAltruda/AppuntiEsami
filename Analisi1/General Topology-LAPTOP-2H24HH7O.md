---
tags: topology
---
*Definizione*: Sia $X$ un insieme non vuoto. Un insieme $\tau$ di sottoinsiemi di $X$ si dice *topologia* su $X$ se:
1.  $X$ e l'insieme vuoto, $\varnothing$, appartengono a $\tau$,
2. unione arbitraria di insiemi di $\tau$ appartiene a $\tau$,
3. intersezione a due a due di sottoinsiemi di $\tau$ appartiene a $\tau$.
Allora la coppia $(X,\tau)$ si dice *spazio topologico*.

*Definizione*: Sia $X$ non vuoto e $\tau=\mathscr{P}(X)$, le parti di $X$. Allora $\tau$ si chiama *topologia discreta* su $X$. Lo spazio associato si chiama spazio discreto.

*Definizione*: Sia $X$ non vuoto e $\tau=\left\{ X,\varnothing \right\}$. Allora $\tau$ si dice *topologia indiscreta*

*Proposizione*: Se $(X,\tau)$ è uno spazio topologico tale che per ogni $x \in X$, il singoletto $\left\{ x \right\}$ è in $\tau$, allora $\tau$ è la topologia discreta.
*Dimostrazione*:
Ricordiamo che ogni insieme è unione di tutti i suoi singoletti, quindi se $S\subset X$: 
$$
S=\bigcup_{x \in S}\left\{ x \right\}.
$$
Questo implica che $S\in \tau. \blacksquare$ 

---
*Definizione*: Sia $(X,\tau)$ uno spazio topologico. Gli elementi di $\tau$ si chiamano *aperti*.

*Definizione*: Sia $(X,\tau)$ uno spazio topologico. Un sottoinsieme $S$ di $X$ si dice essere *chiuso* in $(X,\tau)$ se ha il complementare aperto in $(X,\tau)$.

*Definizione*: Un sottoinsieme $S$ di uno spazio topologico $(X,\tau)$ si dice *clopen* se è sia aperto che chiuso in $(X,\tau)$.

*Corollario*:
1. In ogni spazio topologico $(X,\tau)$, sia $X$ che $\varnothing$ sono clopen,
2. in uno spazio discreto tutti i sottoinsiemi di $X$ sono clopen,
3. in uno spazio indiscreto gli unici clopen sono $X$ e $\varnothing$.

---
*Definizione*: Sia $X$ non vuoto. Una topologia $\tau$ su $X$ si dice *cofinita* se i chiusi di $X$ sono $X$ e tutti i suoi sottoinsiemi finiti, o anche che gli aperti sono $\varnothing$ e tutti i sottoinsiemi di $X$ con un numero finito di complementi.

*Esercizio*: Sia $\tau$ una topologia cofinita su $X$. Se $X$ ha almeno $3$ sottoinsiemi clopen distinti allora $X$ è finito.
*Dimostrazione*:
Siano $a$ il clopen in $X$. Essendo $a$ aperto, ha un numero finito di complementi. Cioè $|X\setminus a|<\infty$. Ora essendo $a$ anche chiuso, questo è finito quindi $$
(X\setminus a)\cup a=X
$$
è finito.

*Definizione*: Sia $(X,\tau)$ uno spazio topologico, questo è detto essere spazio $T_{1}$ se ogni singoletto è chiuso in $(X,\tau)$. 

*Definizione*: Sia $(X,\tau)$ uno spazio topologico, questo è detto essere spazio $T_{0}$ se per ogni coppia di punti distinti $a,b$ in $X$ esiste un aperto che contiene uno e non l'altro.

Ogni spazio $T_{1}$ è anche $T_{0}$.

---
*Definizione*: Un sottoinsieme $S$ di $\mathbb{R}$ si dice aperto nella *topologia euclidea* se ha la seguente proprietà: per ogni $x \in S$, esistono $a,b\in \mathbb{R}$, con $a<b$ tale che $x \in(a,b)\subseteq S$.

*Proposizione*: Un sottoinsieme $S$ di $\mathbb{R}$ è aperto se e solo se è unione di intervalli aperti.

*Definizione*: Sia $(X,\tau)$ uno spazio topologico. Una collezione $\mathcal{B}$ di sottoinsiemi aperti di $X$ si dice *base* per la topologia $\tau$ se ogni aperto è unione dei membri di $\mathcal{B}$.

*Proposizione*: Sia $X$ non vuoto e $\mathcal{B}$ una collezione di sottoinsiemi di $X$. Allora $\mathcal{B}$ è una base per la topologia su $X$ se e solo se $\mathcal{B}$ ha le seguenti proprietà:
1. $X=\bigcup_{B\in \mathcal{B}}$,
2. $\forall B_{1},B_{2} \in \mathcal{B},\,\,B_{1}\cap B_{2}$ è unione di membri di $\mathcal{B}$.
*Dimostrazione*: Per esercizio

*Definizione*: Uno spazio topologico $(X,\tau)$ si dice essere $II-$numerabile (o soddisfare il secondo assioma di numerabilità) se esiste una base $\mathcal{B}$ per $\tau$, dove $\mathcal{B}$ consiste solo di un numero numerabile di insiemi.

*Proposizione*: Sia $(X,\tau)$ uno spazio topologico. Una famiglia $\mathcal{B}$ di sottoinsiemi aperti di $X$ è una base per $\tau$ se e solo se per ogni punto $x$ appartenente ad un qualunque aperto $U$, esiste $B\in \mathcal{B}$ tale che $x \in B\subseteq U$.
*Dimostrazione*: Assumiamo che $\mathcal{B}$ sia una base per $\tau$ e che $x \in U\in \tau$. Dato che $\mathcal{B}$ è base per $\tau$, l'aperto $U$ è unione degli elementi di $\mathcal{B}$; cioè $U=\bigcup_{j\in J}B_{j}$, con i $B_{j}\in \mathcal{B}$, per ogni $j$ in qualche insieme di indici $J$. Ma il fatto che $x \in U$ implica che $x \in B_{j}$, per qualche $j\in J$. Quindi $x \in B_{j}\subseteq U$. 
Adesso invece, assumiamo che per ogni $U\in \tau$ e per ogni $x \in U$, esista un $B\in \mathcal{B}$ con $x \in B\subseteq U$. Dobbiamo mostrare che ogni aperto è unioni di membri di $\mathcal{B}$, sia quindi $V$ un aperto. Per ogni $x \in V$, esiste un $B_{x}\in \mathcal{B}$ tale che $x \in B_{x}\subseteq V$. Chiaramente $V=\bigcup_{x \in V}B_{x}$. $\blacksquare$

*Proposizione*: Sia $\mathcal{B}$ una base per una topologia $\tau$ su $X$. Allora un sottoinsieme $U$ di $X$ è aperto se e solo se per ogni $x \in U$ esiste un $B\in \mathcal{B}$ tale che $x \in B\subseteq U$

*Proposizione*: Siano $\mathcal{B}_{1}$ e $\mathcal{B}_{2}$ basi per le topologie $\tau_{1}$ e $\tau_{2}$, rispettivamente, su un insieme non vuoto $X$. Allora $\tau_{1}=\tau_{2}$ se e solo se:
1. per ogni $B\in \mathcal{B}_{1}$ e per ogni $x \in B$, esiste un $B'\in \mathcal{B}_{2}$ tale che $x \in B'\subseteq B$,
2. per ogni $B\in \mathcal{B}_{2}$ e per ogni $x \in B$, esiste un $B'\in B_{1}$ tale che $x \in B'\subseteq B$.

---
*Proposizione*: Sia $A$ un sottoinsieme di uno spazio topologico $(X,\tau)$. Allora $A$ è chiuso se e solo se $A$ contiene tutti i suoi punti di accumulazione.

*Definizione*: Sia $(X,\tau)$ uno spazio topologico, $N\subset X$ e $p$ un punto di $N$. $N$ si dice essere un *intorno* del punto $p$ se esiste un aperto $U$ tale che $p \in U\subseteq N$.

*Proposizione*: Sia $A$ un sottoinsieme di uno spazio topologico $(X,\tau)$. Un punto $x \in X$ è punto di accumulazione di $A$ se e solo se ogni intorno di $x$ contiene un punto di $A$ diverso da $x$.

---
*Definizione*: Sia $(X,\tau)$ uno spazio topologico, si dice *separabile* se contiene un insieme *denso numerabile*.

---
*Definizione*: Sia $(X,\tau)$ uno spazio topologico. Allora si dice essere *connesso* se gli unici clopen sono $X$ e $\varnothing$.

*Proposizione*: $\mathbb{R}$ è connesso.

---
*Definizione*: Sia $Y$ un sottoinsieme non vuoto di uno spazio topologico $(X,\tau)$. La collezione $\tau_{Y}=\left\{ O\cap Y:O\in \tau \right\}$ di sottoinsiemi di $Y$ è una topologia su $Y$ chiamata *topologia sottospazio*. Il sottospazio $(Y,\tau_{Y})$ è sottospazio di $(X,\tau)$.

*Definizione*: Uno spazio topologico $(X,\tau)$ è $T_{2}$ (o di *Hausdorff*) se comunque scelta una coppia di punti distinti $a,b\in X$ esistono un aperto $U$ e un aperto $V$ tale che $a\in U$, $b\in V$ e che $U\cap V=\varnothing$.

*Definizione*: Uno spazio topologico $(X,\tau)$ si dice essere uno *spazio regolare* se per ogni sottoinsieme chiuso $A$ di $X$ e per ogni punto $x \in X\setminus A$, esistono aperti $U,V$ tali che $x \in U, A\subseteq V$ e $U\cap V=\varnothing$. Se lo spazio è regolare e $T_{1}$ allora si dice essere $T_{3}$.

---
Siano $(X,\tau)$ e $(Y,\tau)$ spazi topologici. Allora sono *omeomorfi* se esiste una funzione $f:X\to Y$ con le seguenti proprietà:
1. $f$ è iniettiva,
2. $f$ è surgettiva,
3. $\forall U\in \tau_{1},f^{-1}(U)\in \tau$,
4. $\forall V\in \tau,f(V)\in \tau_{1}$.
$f$ si dice *omeomorfismo*. Si scrive che $(X,\tau)\simeq (Y,\tau)$.

*Proposizione*: Ogni spazio omeomorfo ad uno spazio connesso è connesso.
In particolare ci sono diverse proprietà preservate dagli omeomorfismi:
1. Cardinalità,
2. $T_{0}$,
3. $T_{1}$,
4. $T_{2}$ (o di Hausdorff),
5. essere uno spazio regolare,
6. $T_{3}$,
7. essere secondo numerabile,
8. essere separabile,
9. essere compatto,
10. essere uno spazio discreto,
11. essere uno spazio indiscreto,
12. possedere una topologia cofinita
13. possedere una topologia chiusa numerabile.

---
*Proposizione*: Un sottospazio di $\mathbb{R}$ è connesso se e solo se è un intervallo.

---
*Lemma*: Sia $f$ una funzione da $\mathbb{R}$ in sé stesso. Allora $f$ è continua se e solo se per ogni $a\in \mathbb{R}$ and per ogni $U$ contenente $f(a)$ esiste un aperto $V$ contenente $a$ tale che $f(V)\subseteq U$.

*Definizione*: Siano $(X,\tau)$ e $(Y,\tau_{1})$ spazi topologici e $f$ una funzione da $X$ in $Y$. Allora $f:(X,\tau)\to (Y,\tau_{1})$ è una *mappa continua* se per ogni $U\in \tau_{1}, f^{-1}(U)\in \tau$

*Proposizione*: Composizione di mappe continue è continua.

*Proposizione*: Siano $(X,\tau)$ e $(Y,\tau_{2})$ spazi topologici e $f$ una funzione da $X$ a $Y$. Allora $f$ è un omeomorfismo se e solo se:
1. $f$ è continua,
2. $f$ è bigettiva,
3. $f^{-1}$ è continua.

*Proposizione*: Siano $(X,\tau)$ e $(Y,\tau_{1})$ spazi topologici e $f:(X,\tau)\to (Y,\tau_{1})$ surgettiva e continua. Se $(X,\tau)$ è connesso, allora lo è anche $(Y,\tau_{1})$.

*Definizione*: Uno spazio topologico $(X,\tau)$ è *connesso per archi* se per ogni coppia di punti $a,b\in X$ esiste una mappa continua $f:[0,1]\to (X,\tau)$, tale che $f(0)=a,\,f(1)=b$. La mappa $f$ è il [[Gruppo fondamentale|cammino]] che unisce $a$ e $b$.

*Proposizione*: Ogni spazio connesso per archi è connesso.
Nota: non è sempre vero il viceversa (serve metrico?)

*Definizione*: Sia $(X,\tau)$ uno spazio topologico e sia $a\in X$. La *componente connessa in $X$ di a*, $C_{X}(a)$, è definita come l'unione di tutti i sottoinsiemi connessi di $X$ che contiene $a$.

---
[[Topologia degli spazi metrici|Spazi Metrici]].

*Definizione*: Sia $(X,\tau)$ uno spazio metrico e $r$ un numero reale positivo. Allora la *palla aperta centrata in $a\in X$ di raggio $r$* è l'insieme $B_{r}(a)=\left\{ x:x \in X\text{ and } d(a,x)<r \right\}$.

*Proposizione*: Sia $(X,d)$ uno spazio metrico. Allora la collezione delle palle aperte in $(X,d)$ è una base per una topologia $\tau$ su $X$.

*Definizione*: Metriche su $X$ si dicono *equivalenti* se inducono la stessa topologia su $X$.

*Proposizione*: Sia $(X,d)$ uno spazio metrico e $\tau$ la topologia indotta su $X$ da $d$. Allora un sottoinsieme $U$ è aperto se e solo se per ogni $a\in U$ esiste $\varepsilon>0$ tale che $B_{\varepsilon}(a)\subseteq U$.

*Proposizione*: Ogni spazio metrico è anche di Hausdorff.

*Definizione*: Uno spazio $(X,\tau)$ si dice *metrizzabile* se esiste una metrica $d$ sull'insieme $X$ con la proprietà che $\tau$ è la topologia indotta da $d$.

*Definizione*: Uno spazio metrico $(X,d)$ si dice *completo* se tutte le [[Successioni||successioni di Cauchy]] in $X$ convergono in $X$.
Ad esempio $\mathbb{R}$ è uno spazio metrico completo.

*Definizione*: Uno spazio topologico $(X,\tau)$ si dice *completamente metrizzabile* se esiste una metrica $d$ su $X$ tale che $(X,d)$ è uno spazio metrico completo.

*Definizione*: Uno spazio topologico $(X,\tau)$ si dice *spazio polacco* se è separabile e completamente metrizzabile.
($\mathbb{R}$ con la distanza usuale è uno spazio polacco)

*Definizione*: Uno spazio topologico $(X,\tau)$ si dice *spazio di Suslin* (o Souslin) se è un Hausdorff ed è immagine di uno spazio polacco attraverso una mappa continua. Se $A$ è un sottoinsieme di uno spazio topologico $(Y,\tau_{1})$ tale che con la topologia indotta $\tau_{2}$, lo spazio $(A,\tau_{2})$ è uno spazio di Suslin, allora $A$ si dice *insieme analitico* in $(Y,\tau_{1})$.

*Definizione*: Siano $(X,d)$ e $(Y,d_{1})$ spazi metrici. Allora $(X,d)$ si dice *isometrico* a $(Y,d_{1})$ se esiste una mappa iniettiva $f:X\to Y$ tale che per ogni $x_{1},x_{2}\in X,\,d(x_{1},x_{2})=d_{1}(f(x_{1}),f(x_{2}))$. Questa mappa si chiama *isometria*.

*Definizione*: Siano $(X,d)$ e $(Y,d_{1})$ spazi metrici e $f$ una mappa da $X$ a $Y$. Sia $Z=f(X)$, $d_{2}$ la metrica indotta su $Z$ da $d_{1}$. Se $f:(X,d)\to (Z,d_{2})$ è un isometria, allora $f$ si dice *embedding isometrico* (o immersione isometrica) di $(X,d)$ in $(Y,d_{1})$.

*Definizione*: Siano $(X,d)$ e $(Y,d_{1})$ spazi metrici e $f$ una mappa da $X$ a $Y$. Se $(Y,d_{1})$ è uno spazio metrico completo, $f:(X,d)\to(Y,d_{1})$ è un embedding isometrico e $f(X)$ è un sottoinsieme denso di $Y$ nell'associato spazio topologico, allora $(Y,d_{1})$ si dice essere il *completamento* di $(X,d)$.

*Proposizione*: Se $(X,d)$ è uno spazio metrico, allora *ammette un completamento*.

*Proposizione*: Siano $(A,d_{1})$ e $(B,d_{2})$ spazi metrici completi. Sia $X$ un sottoinsieme di $(A,d_{1})$, con la metrica indotta $d_{3}$, e sia $Y$ un sottoinsieme di $(B,d_{2})$ con la metrica indotta $d_{4}$. Inoltre, sia $X$ denso in $(A,d_{1})$ e $Y$ denso in $(B,d_{2})$. Se esiste un isometria $f:(X,d_{3})\to(Y,d_{4})$, allora esiste un'isometria $g:(A,d_{1})\to(B,d_{2})$ tale che $g(x)=f(x)$ per ogni $x \in X$.

*Definizione*: Sia $(N,||\cdot||)$ uno spazio vettoriale normato e sia $d$ la metrica associata sull'insieme $N$. Allora $(N,||\cdot||)$ si dice *Spazio di Banach* se $(N,d)$ è uno spazio metrico completo.

---
*Definizione*: Sia $f$ una mappa da $X$ in sé stesso. Allora un punto $x \in X$ si dice *punto fisso* di $f$ se $f(x)=x$.

*Definizione*: Sia $(X,d)$ uno spazio metrico e $f$ una mappa da $X$ in sé stesso. Allora $f$ si dice *mappa contrattiva* se esiste un $r\in(0,1)$ tale che: $$
d(f(x_{1}),f(x_{2}))\leq rd(x_{1},x_{2}),\qquad \forall x_{1},x_{2}\in X.
$$
*Teorema*(Teorema del punto fisso di Banach): Sia $(X,d)$ uno spazio metrico completo e $f$ una mappa contrattiva da $(X,d)$ in sé stesso. Allora $f$ ha esattamente $1$ punto fisso.
*Dimostrazione*: (Sul Jackchan)

---
*Definizione*: Sia $A$ un sottoinsieme di uno spazio topologico $(X,\tau)$. Allora $A$ si dice *compatto* se per ogni insieme $I$ e per ogni famiglia di aperti $O_{i},\,i\in I$, tali che $A\subseteq\bigcup_{i\in I}O_{i}$ esiste una sottofamiglia finita $O_{i_{1}},\dots,O_{i_{n}}$ tale che $A\subseteq \bigcup_{n}O_{i_{n}}$.
Queste due famiglie si dicono rispettivamente *ricoprimento aperto* e *sottoricoprimento finito*.

*Definizione*: $A\subseteq X$ con $(X,\tau)$ spazio topologico si dice compatto se per ogni ricoprimento aperto di $A$ ammette un sottoricoprimento finito. Se $A=X$ allora $(X,\tau)$ si chiama *spazio compatto*.

*Proposizione*: l'intervallo chiuso $[0,1]$ è compatto.

*Proposizione*: Sia $f:(X,\tau)\to (Y,\tau_{1})$ una mappa continua e surgettiva. Se $(X,\tau)$ è compatto allora anche $(Y,\tau_{1})$ lo è.

*Proposizione*: Ogni sottoinsieme chiuso di un compatto è compatto.

*Proposizione*: Un sottoinsieme compatto di un Hausdorff è chiuso.

*Proposizione*: I compatti di $\mathbb{R}$ sono limitati.

*Teorema* (Heine-Borel): Ogni sottoinsieme chiuso limitato di $\mathbb{R}$ è compatto.

*Proposizione*: Ogni compatto di $\mathbb{R}$ è chiuso e limitato.

*Definizione*: Un sottoinsieme $A$ di uno spazio metrico $(X,d)$ si dice limitato se esiste un numero reale $r$ tale che $d(a_{1},a_{2})\leq r$, per ogni $a_{1},a_{2}\in A$.

*Teorema* (Heine-Borel generalizzato): Un sottoinsieme di $\mathbb{R}^{n}, n\geq 1$ è compatto se e solo se è chiuso e limitato.

---
*Definizione*: Siano $(X_1,\tau_1), (X_2,\tau_2),\dots, (X_n,\tau_n)$ spazi topologici. Allora la *topologia prodotto* $\tau$ sull'insieme $X_{1}\times X_{2}\times \cdots\times X_{n}$ è la topologia avente la famiglia $\left\{ O_{1}\times \cdots\times O_{n},\, O_{i}\in \tau_{i},\, i=1,\dots,n \right\}$ come base. L'insieme $X_{1}\times X_{2}\times \cdots\times X_{n}$ con la topologia $\tau$ si dice essere il prodotto degli spazi $(X_1,\tau_1), (X_2,\tau_2),\dots, (X_n,\tau_n)$ ed è denotato come $(X_{1}\times \dots \times X_{n},\tau)$.

*Proposizione*: Siano $\mathcal{B_{1}},\dots,\mathcal{B_{n}}$ basi per gli spazi topologici $(X_1,\tau_1), (X_2,\tau_2),\dots, (X_n,\tau_n)$, rispettivamente. Allora la famiglia di insiemi $\left\{ O_{1}\times\dots\times O_{n}: O_{i}\in \mathcal{B_{i},\, i=1,\dots,n}\right\}$ è una base per la topologia prodotto su $X_1\times\dots\times X_n$.

*Proposizione*: Siano $C_1,\dots, C_n$ chiusi dello spazio topologico $(X_1,\tau_1),\dots,(X_n,\tau_n)$, rispettivamente. Allora $C_1\times\dots\times C_{n}$ è un chiuso dello spazio prodotto $(X_1\times\dots\times X_n,\tau)$.

*Definizione*: siano $\tau_{1}$ e $\tau_{2}$ topologie sull'insieme $X$. Allora $\tau_{1}$ si dice essere *più fine* di $\tau_{2}$ se $\tau_{1}\supseteq \tau_{2}$.
$\mathrm{}$  
*Definizione*: Siano $(X,\tau)$ e $(Y,\tau_{1})$ spazi topologici e $f$ una mappa da $X$ in $Y$. Allora $f$ si dice *mappa aperta* se per ogni $A\in \tau,\,f(A)\in \tau_{1}$. Invece, la mappa $f$ si dice *mappa chiusa* se per ogni chiuso $B\in (X,\tau),\,f(B)$ è chiuso in $(Y,\tau_{1})$.

*Proposizione*: Siano $(X_1,\tau_1),\dots,(X_n,\tau_n)$ spazi topologici e $(X_1\times\dots\times X_n, \tau)$ il loro spazio prodotto.  Per ogni $i \in \left\{ 1,\dots, n \right\}$, sia $p_{i}:X_{1}\times \dots \times X_{n}\to X_{i}$ una proiezione, ovvero, $p_{i}(\langle x_{1},\dots,x_{i},\dots,x_n \rangle)=x_{i}$ per ogni $\langle x_{1},\dots,x_{i},\dots,x_n \rangle\in X_{1}\times\dots \times X_{n}$. Allora:
1. ogni $p_{i}$ è una mappa aperta continua e surgettiva;
2. $\tau$ è la topologia meno fine sull'insieme $X_{1}\times\dots \times X_{n}$ tale che ogni $p_{i}$ è continua.

*Proposizione*: Siano $(X_1,\tau_1),\dots,(X_n,\tau_n)$ spazi topologici e sia $(X_1\times\dots\times X_n, \tau)$ il loro spazio prodotto. Allora ogni $(X_{i},\tau_{i})$ è omeomorfo ad un sottospazio di $(X_1\times\dots\times X_n, \tau)$.
*Corollario*: Per $n \geq 2$, le proiezioni di $\mathbb{R}^{n}\to \mathbb{R}$ sono mappe aperte e continue.
