*Teorema*: $\mathbb{Q}$ è denso in $\mathbb{R}$.
*Dimostrazione*: Ci sono 3 casi da considerare:
1. $0<x<y$;
Per l'assioma di Archimede vale che $\exists n\in N:\, n(y-x)>1$, ma anche $\exists \bar{k}\in \mathbb{N}:\, \bar{k} \frac{1}{n}>x$. Chiaramente $\forall k> \bar{k},\, \frac{k}{n}>x$.
Sia quindi $$
K=max\left\{ k\in N: \frac{k}{n}\leq x \right\} 
$$
Vale che 
$$
\frac{K}{n}<x< \frac{K+1}{n}
$$
$\frac{K+1}{n}=q\in \mathbb{Q}$ .Otteniamo che: $$
x< q= \frac{K+1}{n}= \frac{K}{n}+ \frac{1}{n}< \frac{K}{n}+ (y-x) < x+(y-x)=y
$$
Quindi: $$
x<q<y
$$ come cercato.

2. $x<0<y$;
Il caso è banale dato che $0\in\mathbb{Q}$.

3. $x<y<0$.
Si procede applicando il punto $1$ al caso equivalente $0<-y<-x$. Otterremo così $-q$ che è il numero razionale cercato.