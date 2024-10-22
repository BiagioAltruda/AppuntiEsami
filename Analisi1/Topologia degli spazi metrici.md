---
tags: topology
---



Per il resto del documento, sia $(E,d)$ uno spazio metrico

---
$A \subset E$ si dice essere aperto se $$
\forall x \in A,\exists r>0:\quad B_{r}(x)\subset A
$$
l'insieme di tutti gli aperti si dice *topologia* indotta dalla metrica di $(E,d)$ e si indica con $\tau_{d}$ (o semplicemente $\tau$ se non si rischia confusione).

In seguito indicheremo con $\varepsilon$ la *topologia euclidea* su $\mathbb{R}$, cioè quella indotta dalla metrica euclidea $d(x,y)=|x-y|$.

---
se $x \in E$, si dice intorno di $x$ qualunque insieme $U\subset E$ tale che $$
\exists r>0:\qquad B_{r}(x)\subset U
$$
L'insieme degli intorno di $x$ si indica con $\mathcal{F_{x}}$.

---
*Proposizione A5.2*:
Per gli intorni valgono le seguenti proprietà:
1. ogni punto ha almeno un intorno ed appartiene a tutti i suoi intorni,
2. ogni insieme che contiene un intorno di $x$ è un intorno di $x$,
3. l'intersezione di un numero finito di intorni di $x$ è un intorno di $x$,
4. presi comunque due punti distinti questi possiedono due intorni disgiunti,
5. ogni intorno di $x$ contiene un aperto al quale appartiene $x$.
*Dimostrazione*:
I primi due punti sono ovvi, per il terzo basta considerare che ognuno di questi intorni contiene la palla che ha raggio più piccolo. Per la quarta proprietà osserviamo che $x \neq y$ allora $d(x,y)>0$, quindi posto $r=\frac{d(x,y)}{2}$ abbiamo $B_{r}(x)\cap B_{r}(y)=\varnothing$: se così non fosse, preso $z\in B_{r}(x)\cap B_{r}(y)$ avremmo
$$
d(x,y)\leq d(x,z)+d(z,y)<r+r=d(x,y)
$$
che è assurdo, quindi abbiamo trovato due intorni disgiunti. per quanto riguarda l'ultima proprietà è vera perché basta considerare una palla centrata in $x$ e contenuta in quell'intorno: abbiamo già visto la ogni palla è un aperto. Notiamo che con questa nuova definizione di intorno, se $U\in \mathcal{F_{x}}$ non è vero in generale che $U$ è anche intorno di ogni suo punto: ciò è vero solo se $U$ è un aperto.

---
*Proposizione A5.3*:
In uno spazio metrico $(E,d)$ la topologia $\tau$ ha le seguenti proprietà:
1. il vuoto e tutto lo spazio sono aperti;
2. l'intersezione di un numero finito di aperti è un aperto;
3. l'unione di una famiglia qualsiasi di aperti è un aperto;
4. presi comunque due punti distinti di $E$ questi sono contenuti in due aperti disgiunti.

---
Si dice che $C\subset E$ è chiuso se il suo complementare $E\setminus C$ è aperto.

Se $B\subset E$, l'interno $\dot{B}$ di $B$ è il più grande aperto contenuto in $B$, e la chiusura $\bar{B}$ di $B$ è il più piccolo chiuso contenente $B$, cioè, posto $$
\alpha=\left\{ A\subset B:A\in\tau \right\},\qquad \gamma =\left\{ C \supset B:E\setminus C\in\tau\right\},  
$$
si ha $$
\dot{B}=\bigcup_{A\in \alpha}A,\qquad \bar{B}=\bigcap_{C\in\gamma}C.
$$
Infine, il bordo di $B$ è $\partial B=\bar{B}\setminus \dot{B}$

---
Un insieme $D\subset E$ si dice denso in $E$ se $\bar{D}=E$
*Proposizione A5.4*:
la chiusura è involutoria, cioè per ogni $B\subset E$ si ha $\bar{\bar{B}}=B$
inoltre per ogni $A,B \subset E$ si ha $\overline{A\cup B} =\bar{A}\cup \bar{B}$
*Proposizione A5.5*:
per ogni $B\subset E$ si ha che $\dot{B}=(\overline{B^{c}})^{c}$.
*Proposizione A5.6*: l'interno di $A\cap B$ è uguale ad $\dot{A}\cap \dot{B}$

---
Un insieme $\mathcal{B_{x}}\subset \mathcal{P}(E)$ si dice base degli intorni di un punto $x$ se valgono le seguenti proprietà:
1. ogni elemento di $\mathcal{B_{x}}$ è intorno di $x$;
2. ogni intorno di $x$ contiene qualche elemento di $\mathcal{B_{x}}$
#topology 