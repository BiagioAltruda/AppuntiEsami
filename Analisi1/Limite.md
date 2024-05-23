Diciamo che la [[Successioni|successione]] $\{a_n\}_n$ ammette *limite* $l\in\bar{\mathbb{R}}$ (i numeri reali estesi) o più brevemente, tende ad $l$, se:
$$\forall U\in\mathcal{F}_l,\,\exists\bar{n}\in\mathbb{N}:\forall n\geq\bar{n},\quad a_n\in U$$
in tal caso scriviamo $a_n\to l$

---
*Teorema 5.12* :
Il limite di una successione, se esiste, è unico.
*Dimostrazione*:
se $a_n\to l_1$ e $a_n\to l_2$ con $l_1\neq l_2$, possiamo scegliere due intorni disgiunti $U_1\in\mathcal{F}_{l_1}$ e $U_2\in\mathcal{F}_{l_2}$. Per la definizione di limite, definitivamente $a_n\in U_1$ e $a_n\in U_2$ cioè definitivamente $a_n\in U_1\cap U_2$, che è assurdo essendo loro disgiunti. $\blacksquare$

---
*Proposizione 5.13*:
Se $a_n\to l$ allora ogni sua estratta tende a $l$.
*Dimostrazione*:
Sia $\{a_{n_k}\}_n$ un estratta, allora:
$$n>\bar{n}\Rightarrow k_n\geq n\geq \bar{n}$$
dunque:
$$\forall n\geq\bar{n},\quad a_k\in U$$
$\blacksquare$

---
*Proposizione 5.16*:
Una successione $\{a_n\}_n$ converge ad $l\in\mathbb{R}$ se e solo se: $$\forall\varepsilon>0\,\exists\bar{n}:\forall n\geq\bar{n}, \quad |a_n-l|<\varepsilon$$
Una successione $\{a_n\}_n$ diverge positivamente (negativamente) se e solo se: $$\forall M\,\exists\bar{n}\geq n,\quad a_n>M\quad(<M)$$
La prima proprietà è equivalente a dire che:
$$\forall\varepsilon>0,\exists\bar{n}:\forall n\geq \bar{n}, l-\varepsilon<a_n<l+\varepsilon$$

---
*Teorema 5.25*:
Siano $\{a_n\}_n$ e $\{b_n\}_n$ due successioni tali che $$a_n\to l_a,\qquad b_n\to l_b$$
Allora, se ha senso scrivere $l_a+l_b$, abbiamo $$(a_n+b_n)\to(l_a+l_b).$$
E vale lo stesso per il prodotto, se ha senso.
*Dimoostrazione*:
Iniziamo con il caso $l_a,l_b\in\mathbb{R}$: fissato $\varepsilon>0$, abbiamo definitivamente $$|a_n-l_a|<\varepsilon,\quad|b_n-l_b|<\varepsilon$$
Per disuguaglianza triangolare otteniamo: $$|(a_n+b_n)-(l_a+l_b)|=|(a_n-l_a)+(b_n-l_b)|\leq |a_n-l_a|+|b_n-l_b|$$
Quindi definitivamente: $$|(a_n+b_n)-(l_a+l_b)|<2\varepsilon$$
Supponiamo adesso il caso $l_a=+\infty$ quindi $l_b$ può essere o no $+\infty$ ma in ogni caso è inferiormente limitato. In particolare $b_n$ converge o diverge positivamente. Vale a dire: $$\exists K\in\mathbb{R}:\forall n\in\mathbb{N},\quad b_n\geq K$$ (è limitata inferiormente), quindi $$a_n+b_n\geq a_n+K$$
poiché $a_n\to+\infty$, per ogni $M\in\mathbb{R}$ definitivamente $a_n>M$, quindi $$a_n+b_n>M+K$$ dunque $$(a_n+b_n)\to+\infty$$Passiamo a dimostrare il caso del prodotto dato che gli altri casi della somma sono analoghi. Iniziamo col caso reale. osserviamo che:$$|a_nb_n-l_al_b|=|a_nb_n-l_ab_n+l_ab_n-l_al_b|\leq|a_n-l_a|\cdot|b_n|+|l_a|\cdot|b_n-l_b|$$
Dato che $\{b_n\}_n$ converge, è limitata, pertanto esiste $K>0$ tale che per ogni $n$ si ha che $|b_n|\leq K$, scelto $\varepsilon>0$, per ipotesi definitivamente vale: $$|a_nb_n-l_al_b|\leq |a_n-l_a|\cdot|b_n|+|l_a|\cdot|b_n-l_b|\leq K\varepsilon+|l_a|\varepsilon\leq (K+|l_a|)\varepsilon$$
Non ci rimane che il caso $l_a=+\infty$ e $l_b>0$. Scelto un numero $K\in(0,l_b)$, per esempio $K=\frac{l_b}{2}$m se $l_b\in\mathbb{R}$, o $K=1$ se $l=+\infty$ , definitivamente $b_n\geq K$, d'altra parte, fissato $M>0$, definitivamente $a_n>M$, quindi $a_nb_n>KM$ cioè $a_nb_n\to+\infty = l_al_b.\,\,\,\blacksquare$ ^a4cf4b

---
*Proposizione 5.27*:
Il prodotto di una successione infinitesima per una limitata è una successione infinitesima.
*Dimostrazione*:
Se $a_n\to 0$ allora anche $|a_n|\to0$, mentre se $\{b_n\}_n$ è limitate esiste $K>0$ tale che $\forall n\in\mathbb{N}\quad|b_n|\leq K$. Allora $$0\leq|a_nb_n|=|a_n||b_n|\leq K|a_n|,$$ dato che $K|a_n|\to 0$, anche $|a_nb_n|\to 0$ per il teorema dei carabinieri, quindi $a_nb_n\to0$ per la caratterizzazione sui moduli delle successioni (Proposizione 5.18) [[Successioni#^9be3a8| Proposizione 5.18]]. $\blacksquare$ 

---
*Proposizione 5.29*:
Se $a_n\to l$ allora anche $|a_n|\to l$
*Dimostrazione*:
Cominciamo con il caso $l\in\mathbb{R}$, per disuguaglianza triangolare vale: $$0\leq||a_n|-|l||\leq|a_n-l|$$ d'altra parte $a_n\to l$ quindi $(a_n-l)\to 0$ quindi anche $|a_n-l|\to 0$, si conclude applicando il [[Teoremi di confronto per successioni#^5ede27|teorema dei carabinieri]].
Il caso $l=\pm \infty$ è triviale.

---
*Proposizione 5.30*:
Siano $a_{n}\to l$ e $b_{n}\to l$ due successioni:
1. se $l_{a}<l_{b}$ allora definitivamente $a_{n}<b_{n}$,
2. se [[definitivamente e frequentemente|frequentemente]] $a_{n}\leq b_{n}$ allora $l_{a}\leq l_{b}$.

---
*Proposizione 5.31*:
se $a_{n}\to l$ allora: $$
l=+\infty \Rightarrow \frac{1}{a_{n}}\to 0^{+}
$$$$
l\in\mathbb{R}\setminus \left\{ 0 \right\} \Rightarrow \frac{1}{a_{n}} \to \frac{1}{l}   
$$
$$l=0^{+} \Rightarrow \frac{1}{a_{n}} \to +\infty$$
Se $a_{n}$ ha segno [[definitivamente e frequentemente|definitivamente]] non costante, allora $\left\{ \frac{1}{a_{n}} \right\}_{n}$ non ha limite.
Valgono le proposizioni analoghe con $0^{-}$ e $-\infty$.

*Dimostrazione*:
Per il [[Limite#^a4cf4b|teorema sul limite del prodotto]] basta considerare i casi $l=+\infty$, $l=0^{+}$,  $0<l<+\infty$, dato che gli altri si ottengono applicando questo risultato alla successione $\left\{ -a_{n} \right\}_{n}$. In ciascuno di questi casi, definitivamente $a_{n}>0$, pertanto anche $\frac{1}{a_{n}}>0$.
Iniziamo con $l=+\infty$: scelto $\varepsilon>0$, definitivamente $a_{n}>\frac{1}{\varepsilon}$, quindi definitivamente: $$
-\varepsilon<0< \frac{1}{a_{n}}<\varepsilon
$$
cioè $\frac{1}{a_{n}}\to 0^{+}$.

Caso $l=0^{+}$: se $a_{n}\to l=0^{+}$ sia $(H,K)$ un intorno di $l$, vale che $0\leq H<a_{n}<K$ vale a dire che $\frac{1}{K} < \frac{1}{a_{n}}< \frac{1}{H}\leq+\infty$. Chiaramente $\frac{1}{K}\to +\infty\Rightarrow \frac{1}{a_{n}}\to +\infty$.

Caso $0<l<+\infty$: Fissato un intorno $(H,K)$ di $\frac{1}{l}$, scegliamo $H'\geq H$ in modo che $0<H'< \frac{1}{l}$. Allora abbiamo $0< \frac{1}{K}<l< \frac{1}{H'}$, quindi  definitivamente $0< \frac{1}{K}<a_{n}< \frac{1}{H'}$ vale a dire $H'< \frac{1}{a_{n}} <K$, pertanto $H< \frac{1}{a_{n}}< K$, che dimostra $\frac{1}{a_{n}}\to \frac{1}{l}.\,\,\blacksquare$ 

---
**Limiti di Funzioni**
I limiti di funzioni si definiscono come: $$
\lim_{ x \to +\infty }f(x)=l \Leftrightarrow \forall U\in \mathcal{F}_{l},\exists\bar{x}\in \mathbb{R}:\forall x\in (\text{dom}f)  \cap [\bar{x},+\infty[,\qquad f(x)\in U.
$$
---
Sia $f$ una funzione reale tale che $+\infty$ è punto di accumulazione del dominio di $f$; diciamo che $f$ tende a $l\in\bar{\mathbb{R}}$ per $x\to +\infty$ se: $$
\forall U\in \mathcal{F}_{l},\exists\bar{x}\in \mathbb{R}:\forall x\in (\text{dom}f)  \cap [\bar{x},+\infty[,\qquad f(x)\in U.
$$
In tal caso scriviamo $$
\lim_{ x \to +\infty }f(x)=l 
$$
Valgono le proprietà:
1. $$
\lim_{ x \to +\infty }f(x)=l \Leftrightarrow \forall U\in \mathcal{F}_{l},\exists\bar{x}\in \mathbb{R}:\forall x\in \text{dom}f,\qquad x\geq \bar{x} \Rightarrow f(x)\in U
$$ $$
	\Leftrightarrow \forall U\in\mathcal{F_{l}},\exists \bar{x} \in \mathbb{R}: \forall x\in \text{dom}f, \qquad x> \bar{x} \Rightarrow f(x)\in U
$$
2. $$\lim_{ x \to +\infty }f(x)=+\infty \Leftrightarrow \forall M\in \mathbb{R},\exists  \bar{x} \in \mathbb{R} : \forall x \in \text{dom}f,\quad x> \bar{x}\Rightarrow f(x) > M$$
3. 
$$\lim_{ x \to +\infty }f(x)=l\in \mathbb{R} \Leftrightarrow \forall U\in \mathcal{F}_{l},\exists\bar{x}\in \mathbb{R}:\forall x\in \text{dom}f,\qquad x \geq \bar{x} \Rightarrow l-\varepsilon<f(x)<l+\varepsilon$$
Analoghe per $x \to -\infty$.

---
Sia $f$ una funzione reale, e sia $x_{*}$ un suo punto di accumulazione. Diciamo che la funzione $f$ tende a $l\in \mathbb{R}$ per $x$ che tende a $x_{*}$  se $$
\forall U \in \mathcal{F_{l}}, \exists V \in \mathcal{F_{x_{*}}}:\forall x\in \text{dom}f \cap V\setminus \left\{ x_{*} \right\}, \qquad f(x)\in U 
$$
In tal caso scriviamo $\lim_{ x \to x_{*} }=l$ 
Valgono le analoghe proprietà dei limiti di [[Teoremi di confronto per successioni#^04236a|successioni]].

---
	*Teorema 6.2*: se $f$ è una funzione reale, e $x_*$, è un punto di accumulazione di dom$f$, allora sono equivalenti:
1. $\lim_{ x \to x_{*} }=l$
2. per ogni successione $\left\{ x_{n} \right\}_{n}$ di punti in $\text{dom}f\setminus \left\{ x_{*} \right\}$, se $x_{n}\to x_{*}$ allora $f(x_{n})\to l$.
*Dimostrazione*: iniziamo con $1)\Rightarrow 2)$; Sia dunque $\left\{ x_{n} \right\}_{n}$ una successione di punti del dominio di $f$, diversi da $x_{*}$, che tende ad $x_{*}$ e fissiamo un intorno $U\in \mathcal{F_{l}}$ dobbiamo provare che definitivamente $f(x_{n})\in U$. Sappiamo che esiste un intorno $V\in\mathcal{F_{x_{*}}}$ tale che se $x\in \text{dom}f \cap V\setminus \left\{ x_{*} \right\}$ allora $f(x)\in U$, ma $x_{n}\to\in \text{dom}f\setminus \left\{ x_{n} \right\}_{n}$ per ogni $n$, per ipotesi, e definitivamente $x_{n}\in V$ perché $x_{n}\to x_{*}$ e $V$ è un intorno di $x_{*}$, dunque definitivamente $x_{n}\in \text{dom}f\cap V\setminus \left\{ x_{n} \right\}_{n}$ così definitivamente $f(x_{n})\in U$, come richiesto.
Dimostriamo adesso $2)\Rightarrow 1)$. supponiamo che non sia vero che $f(x)\to l$, e mostriamo che esiste una successione $\left\{ x_{n} \right\}+n$ di punti del dominio di $f$ diversi da $x_*$ che tende a $x_{*}$ e tale che $\left\{ f(x_{n}) \right\}_{n}$ non tende ad $l$. Ovvero:
$$
\exists U_{0}\in\mathcal{F_{l}}:\forall V\in\mathcal{F_{x_{*}}}, \exists x\in \text{dom}f \cap V\setminus \left\{ x_{n} \right\}: f(x)\not\in U_{0}
$$ Scegliamo una successione $\left\{ V_{n} \right\}_{n}$ di intorni di $x_{*}$ come segue: $$
\text{se } x_{*}=+\infty,\qquad V_{n}=(n,+\infty)
$$
$$
\text{se } x_{*} \in \mathbb{R}\qquad V_{n}=\left( x_{*}-\frac{1}{n}, x_{*}+ \frac{1}{n} \right)
$$
$$
\text{se }x_{*}=-\infty,\qquad V_{n}=(-\infty,n)
$$
Osserviamo che per il teorema dei carabinieri se $\left\{ x_{n} \right\}_{n}$ è una qualsiasi successione tale che $\forall n,x_{n}\in V_{n}$ allora $x_{n}\to x_{*}$. Segue anche per ogni $n$ esiste un punto, $x_{n}$, tale che $x_{n}\in \text{dom}f\cap V_{n}\setminus \left\{ x_{n} \right\}$ e che $f(x_{n})\notin U_{0}$, che è assurdo. $\blacksquare$

---
Seguono alcuni *limiti fondamentali*:
$$
\begin{gather}
 \lim_{ x \to 0 } \frac{\sin x}{x}=1, \qquad 6.9)\\
 \lim_{ x \to 0 } \frac{1-\cos x}{x^{2}}=\frac{1}{2},\qquad 6.10)\\
 \lim_{ x \to 0 } \frac{e^x-1}{x}=1, \qquad 6.11)\\
 \lim_{ x \to 0 } \frac{\log(1+x)}{x}=1,\qquad 6.12)\\
 \lim_{ x \to  \pm \infty} \left(1+\frac{1}{x}\right)^{x}=e\qquad 6.13),\\
 \lim_{ x \to 0 } (1+x)^{1/x}=e, \qquad 6.14)
\end{gather}
 $$
 e anche $$
\begin{gather}
\lim_{ x \to -\infty } e^{x}=0^{+},\quad\lim_{ x \to \infty } e^{x}=+\infty\quad 6.15)\\
\lim_{ x \to 0^{+} } \log x=-\infty,\quad\lim_{ x \to +\infty }\log x=+\infty\quad 6.16) 
\end{gather}
$$

#SuccessionieSerie 
#Limiti

^7fd831


^604ab5
