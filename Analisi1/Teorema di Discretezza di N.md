*Teorema*: $\forall n\in \mathbb{N}:\, (n,n+1)\cap \mathbb{N}=\varnothing$.
*Dimostrazione*: Sia $C=\left\{ n\in \mathbb{N}|(n,n+1)\cap \mathbb{N}=\varnothing \right\}\subset \mathbb{N}$. Proviamo che $C$ è induttivo.
1. $0\in C\,$? Sia $A=\mathbb{N}\setminus(0,1)\subset \mathbb{N}$. Proviamo che $A$ è induttivo. $0\in \mathbb{N},\, 0\not\in(0,1)\Rightarrow 0\in A$. inoltre sia $n\in A$.
$$
n \geq 0\Rightarrow n+1\geq 1\Rightarrow n+1 \not\in(0,1)\Rightarrow n+1\in A
$$
Quindi $A$ è induttivo. Per il principio di induzione $A=\mathbb{N}$.
Quindi $\mathbb{N}\setminus (0,1)=\mathbb{N}\Leftrightarrow \mathbb{N}\cap(0,1)=\varnothing$.
Quindi $0\in C$.

2. Sia $n\in C$. Mostriamo che $n+1\in C$.
$$
n\in C\Leftrightarrow(n,n+1)\cap \mathbb{N}=\varnothing
$$
Poniamo
$$
B=\mathbb{N}\setminus(n+1,n+2)\subset \mathbb{N}
$$
Proviamo che $B$ è induttivo.
$0\in B$ poiché $\forall n\in \mathbb{N}:\, n+1>0 \text{ e } 0\not\in(n+1,n+2)\Rightarrow 0\in B$. Sia $m\in \mathbb{N}$, suppongo $m\in B \Leftrightarrow m\in \mathbb{N}\setminus(n+1,n+2)$. Quindi $m\leq n+1 \vee n\geq n+2$.
	2.1 $m<n+1$. dato che $(n,n+1)\cap \mathbb{N}=\varnothing$, si ha che $m\leq n$. Segue che $m+1<n+1\Rightarrow m+1\in B$.
	2.2 $m=n+1\Rightarrow m+1=n+2 \not\in(n+1,n+2)\Rightarrow m+1\in B$.
	2.3 $m\geq n+2\Rightarrow m+1\geq n+3\Rightarrow m+1\in B$.
Segue che $B$ è induttivo e che $B=\mathbb{N}$. Quindi $\mathbb{N}\cap(n,n+1)=\varnothing$, quindi $C$ è induttivo e $C=\mathbb{N}$.
Da cui $\mathbb{N}\cap(n,n+1)=\varnothing,\quad\forall n\in \mathbb{N}$.