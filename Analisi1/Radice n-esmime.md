Sia $n\in\mathbb{N}^+$, $z$ un [[Numeri Complessi|numero complesso]] si dice *radice $n$-esima* di $w$ se $z^n=w$
*Teorema*: Per ciascun valore di $n\in\mathbb{N}^+$, ogni numero complesso diverso da $0$ ha esattamente $n$ radici $n$-esime distinte.
*Dimostrazione*:
se $z$ è una radice $n$-esima di $w$ allora $z^n=w$, allora anche $|z^n|=|w|\Rightarrow |z|^n=|w|\Rightarrow |z|=\sqrt[n]{|w|}$
se $w\neq 0$ scrivo $z$ e $w$ in forma trigonometrica: 
$$z=\rho(\cos\theta+i\sin\theta),\qquad w=r(\cos\theta+i\sin\theta)$$
Da cui ricaviamo: 
$$\rho^n(\cos(n\theta)+i\sin(n\theta))=r(\cos\phi+i\sin\phi)$$
da $\rho^n=r\neq0$ otteniamo l'equazione: 
$$\cos(n\theta)+i\sin(n\theta)=\cos\phi+i\sin\phi$$
che equivale al sistema: $$\begin{align*}\cos(n\theta)=cos\phi \\\sin(n\theta)=\sin\theta\end{align*}$$
$n\theta$ e $\phi$ differiscono per un multiplo intero di $2\pi$: $$n\theta=\phi+2m\pi$$
Ovvero: $$\theta=\frac{\phi}{n}+\frac{2m\pi}{n}$$
[[Algoritmo di Bezout|Dividendo]] l'intero $m$ per l'intero $n$ troviamo $h,k$ tali che: 
$$m=hn+k,\qquad k\in\{0,\dots,n-1\}$$
Segue che: $$\theta=\frac{\phi}{n}+2m\pi+\frac{2k\pi}{n}$$
Considerando $\theta$ come l'argmin, possiamo ignorare $2m\pi$. Poniamo: 
$$\begin{align}\theta_0=\frac{\phi}{n}\\\theta_1=\frac{\phi}{n}+\frac{2\pi}{ n}\\\vdots\\\theta_{n-1}=\frac{\phi}{n}+\frac{2(n-1)\pi}{n}\end{align}$$
.Vale quindi che per ogni $k\in\{0,\dots,n-1\}$:
$$z_k=\sqrt[n]{r}(\cos\theta_k+i\sin\theta_k)$$
Questi $n$ numeri hanno tutti argomenti diversi e compresi in $[0,2\pi]$ quindi sono tutti distinti. $\blacksquare$ 
#complex