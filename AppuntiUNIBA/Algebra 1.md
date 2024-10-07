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
(x*y)*(\bar{y}*\bar{x})=x*(y*(\bar{y}*\bar{x}))=x*((y*\bar{y})*\bar{x})=x*(e*\bar{x})=
$$