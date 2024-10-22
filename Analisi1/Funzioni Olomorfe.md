*Definizione*(funzione olomorfa):
Siano $U\subseteq \mathbb{C}$ un aperto, $z_{0}\in U$ e $f:U\to \mathbb{C}$. La funzione $f$ si dice olomorfa (o derivabile in senso complesso) in $z_{0}$ se il seguente limite esiste $$
\lim_{ z \to z_{0} } \frac{f(z)-f(z_{0})}{z-z_{0}}=f'(z_{0})\in \mathbb{C}.
$$
$f$ è olomorfa se lo è in $z_{0}$ per ogni $z_{0}\in U$.
Poniamo
$$
\mathcal{O}(U)=\left\{ f:U\to \mathbb{C}|f \text{ è olomorfa} \right\} 
$$
---
Le condizioni di essere differenziabile ed essere olomorfa sono leggermente diverse come mostrato nella proposizione successiva.
*Proposizione* (caratterizzazione delle funzioni olomorfe):
Sia $f:U\to \mathbb{C}$ con $U$ aperto e $z_{0}\in U$. Le seguenti affermazioni sono equivalenti:
1. $f$ è olomorfa in $z_{0}$;
2. $f$ è differenziabile in $z_{0}$ e $df_{z_{0}}$ è $\mathbb{C}-$lineare;
3. $f$ è differenziabile in $z_{0}$ e $\frac{ \partial f }{ \partial \bar{z} }(z_{0})=0$;
4. $f$ è differenziabile e valgono le equazioni di Cauchy-Riemann, cioè
$$
\frac{ \partial \mathfrak{Re}(f) }{ \partial x }=\frac{ \partial \mathfrak{Im}(f) }{ \partial y }, \qquad \frac{ \partial \mathfrak{Re}(f) }{ \partial y }=-\frac{ \partial \mathfrak{Im}(f) }{ \partial x };   
$$
5. $df_{z_{0}}(w)=f'(z_{0})w$.

---
*Teorema*(Proprietà aritmetiche delle funzioni olomorfe):
Siano $f:U\to \mathbb{C}$ e $g:V\to \mathbb{C}$ olomorfe. Allora
1. se $U=V$ allora $f+g:U\to \mathbb{C}$ è olomorfa;
2. se $U=V$ allora $fg:U\to \mathbb{C}$ è olomorfa e $$
(fg)'=f'g+fg'
$$
3. se $f(U)\subseteq V$ allora $g\circ f:U\to \mathbb{C}$ è olomorfa e $$
(g\circ f)'(z_{0})=g'(f(z_{0}))f'(z_{0})
$$
4. se $f'(z_{0})\neq 0$ e $f\in C^{1}$ allora esistono un intorno $W$ di $f(z_{0})$ in $\mathbb{C}$ e un intorno $Z$ di $z_{0}$ in $U$ tali che $f(Z)-W,\,\,f_{|_{Z}}\to W$ è bigettiva e $(f_{|_{ }})^{-1}:W\to Z$ è olomorfa con $$
((f_{|_{Z}})^{-1})'(f(z_{0}))=\frac{1}{f'(z_{0})}
$$
---
*Proposizione*(Inversa moltiplicativa di olomorfa è olomorfa):
Sia $f:U\to \mathbb{C}$ olomorfa in $z_{0}$ e $f(z_{0})\neq 0$ allora $1\setminus f$ è olomorfa in $z_{0}$ e $$
\left( \frac{1}{f} \right)'(z_{0})=\frac{f'(z_{0})}{f(z_{0})^{2}}
$$

## Funzioni analitiche
Studiamo una classe di funzioni più piccola delle olomorfe. Mostreremo che le analitiche da $U\subseteq \mathbb{C}$ aperto a $\mathbb{C}$ sono esattamente le funzioni olomorfe.

*Definizione*(Serie di potenze):
Una serie della forma $$
\sum_{n=0}^\infty a_{n}(z-z_{0})^{n}
$$
è detta serie di potenze di centro $z_{0}$.
Una serie di potenze ammette un *raggio di convergenza*, cioè esiste $R>0$ tale che la serie converge assolutamente in $B_{R}(z_{0})$ e diverge in $C\setminus\overline{B_{R}(z_{0})}$.
*Definizione*(funzione analitica):
una funzione $f:U\to \mathbb{C}$ si dice analitica se per ogni $z_{0}\in U$ esiste $R>0$ tale che $f$ sia esprimibile come serie di potenze centrata in $z_{0}$ per ogni $z\in B_{R}(z_{0})$.
*Proposizione*:
Una funzione $f:U\to \mathbb{C}$ analitica è continua.
*Teorema*(Le serie di potenze sono analitiche):
Supponiamo che $$
f(z)=\sum_{n=0}^{\infty}a_{n}(z-z_{0})^{n}
$$
per ogni $z\in B_{R}(z_{0})$ con $R>0$. Allora $f$ è analitica su $B_{R}(z_{0}).$

---
*Teorema*(Serie derivata):
se $f$ è una serie di potenze su $B_{R}(z_{0})$ allora $f$ è olomorfa su $B_{R}(z_{0})$ e $$
f'(z)=\sum_{n=1}^{\infty} a_{n}n(z-z_{0})^{n-1} \text{ per ogni } z\in B_{R}(z_{0})
$$
*Corollario*:
Una funzione analitica complessa è $C^{\infty}$ in senso complesso. (Cioè olomorfa)
*Corollario*(Serie di Taylor):
L'espressione di $f$ come serie di potenze è unica:$$
f(z)=\sum_{n=0}^{\infty} \frac{f^{(n)}(z_{0})}{n!}(z-z_{0})^{n}
$$
*Corollario*:
composizione di funzioni analitiche è analitica

## Ordine di annullamento

Studiamo come si comportano gli zeri delle funzioni analitiche

*Definizione* (ordine di annullamento):
Sia $f:U\to \mathbb{C}$ olomorfa. L'ordine di annullamento (o di svanimento o di zero) di $f$ in $z_{0}$ è dato da $$
\begin{cases}
\min\left\{ n\in \mathbb{N}|f^{(n)}(z_{0})\neq0 \quad\text{se }\exists n\in \mathbb{N}\text{ tale che }f^{(n)}(z_{0})\neq 0 \right\} \\ \\
\infty\qquad\qquad\qquad\qquad\qquad\,\,\, \text{altrimenti}
\end{cases}
$$
Osserviamo che $f$ ha ordine di annullamento $0$ se $f(z_{0})\neq 0$ e ha ordine $\geq1$ se $f(z_{0})=0$.
*Lemma* (Caratterizzazione dell'ordine di annullamento):
sia $f$ analitica (e quindi olomorfa). Le seguenti proposizioni sono equivalenti:
1. $z_{0}$ ha ordine di annullamento $n_{0}$ per $f$;
2. $f(z)=(z-z_{0})^{n_{0}}g(z)$ in un intorno di $z_{0}$ con $g(z_{0})\neq 0$ e $g$ analitica.
*Lemma*:
Sia $f:U\to \mathbb{C}$ analitica e sia $Z=\left\{ z_{0}\in U|f(z_{0}=0) \right\}$. Sia $z_{0}\in Z$. Si ha che $z_{0}$ è un punto isolato di $Z$ o $z_{0}\in \dot{Z}$ (La parte interna di $Z$)

---
*Teorema*(gli zeri di una funzione analitica sono isolati o coprono la componente connessa):
Sia $F:U\to \mathbb{C}$ analitica con $U$ *connesso*. Supponiamo che $Z=f^{-1}(0)\subseteq U$ abbiamo un punto di accumulazione in $U$. Allora $f=0$ come funzione su $U$
*Dimostrazione*:
Poiché $\tilde{z}$ è di accumulazione si ha che esiste una successione $\left\{ z_{n} \right\}\subseteq U$ tale che $z_{n}\to \tilde{z}\in U$, $z_{n}\neq \tilde{z}$ e $f(z_{n})= 0$ per ogni $n$. Per la continuità di $f$ si ha che $$
f(\tilde{z})=f(\lim_{ n \to \infty } z_{n})=\lim_{ n \to \infty } f(z_n)=\lim_{ n \to \infty } 0=0,
$$
perciò $Z=f^{-1}(0)\supseteq \left\{ z_n \right\}\cup \left\{ \tilde{z} \right\}$. Per costruzione $\tilde{z}$ non è uno zero isolato, quindi abbiamo che $\tilde{z}\in \dot{Z}\neq \varnothing$. Essendo $U$ *connesso*, basta mostrare che la parte interna di $Z$ è sia aperta che chiusa. la parte interna di $Z$ è aperta per definizione di parte interna. Mentre per mostrare che è chiusa, se per assurdo $w\in\overline{\dot{Z}}\setminus \dot{Z}$ allora esisterebbe una successione $w_{n}\in \dot{Z}$ con $w_{n}\to w$ e $w_{n}\neq w$ (cioè $w\not\in \dot{Z}$). Allora avremmo $f(w)= 0$ per continuità, in particolare $w$ è uno zero non isolato. e cioè $w \in \dot{Z}$, che contraddice le ipotesi. $\blacksquare$

Che si riformula nel potente *corollario*(Principio di identità per analitiche):
Se $U$ è connesso e $f,g:U\to \mathbb{C}$ sono analitiche e $W\subseteq U$ contiene un punto non isolato allora $f=g$ su $U$ se e solo se $f=g$ su $W$.

---
[[Esponenziale e logaritmo complessi]]


#complex 