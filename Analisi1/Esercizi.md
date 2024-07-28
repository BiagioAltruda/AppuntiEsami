1. Sia $\delta>0$. Dimostrare l'esistenza di una funzione continua $f$, tale che $supp(f)\subset[2-\delta,2]$ e che: $$
I=\frac{1}{2\pi}\int_{2-\delta}^2f(x)\sqrt{ 4-x^2 }\,dx=1
$$
*Dimostrazione*:
Essendo $f$ continua e a supporto compatto su $[2-\delta,2]$, per l'arbitrarietà di $\delta$ posso scrivere:$$
I=\frac{1}{2\pi}\int_{2-\delta}^2C\sqrt{ 4-x^2 }\,dx
$$
Con $C=f(2)$. Che implica
$$
I=\frac{C}{2\pi}\int_{2-\delta}^2\sqrt{ 4-x^2 }\,dx
$$
Che per un'opportuna scelta di $C$, è uguale ad $1$. $\blacksquare$
2. 
$$x=\sum_{g\in G} g=\sum_{g\in G|o(g)=2}g$$
Se ci sono $4$ elementi di ordine $2$ allora: $$
x=g_{1}g_{2}g_{3}g_{4}=g_{1}g_{2}g_{3}x\Rightarrow e=g_{1}g_{2}g_{3}\Rightarrow g_{1}g_{2}=g_{3}
$$
3.$\forall n\in N,\,\,\mathbb{R}^{n}$ è uno spazio polacco.
*Dimostrazione*: Uno spazio metrico si dice polacco se è separabile e completamente metrizzabile. $\mathbb{R}^{n}$ con la metrica indotta dalla distanza euclidea è uno spazio metrico completo per ogni $n$, dato che se prendiamo una successione di Cauchy in ogni coordinata questa converge. Basta mostrare che $\mathbb{R}^{n}$ è separabile per ogni $n$. Uno spazio è separabile se contiene un denso numerabile. $\mathbb{Q}^{n}\subset \mathbb{R}^{n},\,\forall n\in N$ è un insieme numerabile e denso in $\mathbb{R}^{n}$.

4. Dare un esempio di una successione in $\mathbb{R}$ con la metrica euclidea che non ha sottosuccessioni di Cauchy.
*Dimostrazione*: $x_1=1,x_n=2x_{n-1}$ è una successione monotona crescente, illimitata, quindi non converge e non è di Cauchy, tutte le sue sottosuccessioni sono anche loro monotone crescenti e illimitate.

5. Sia $(X,d)$ uno spazio metrico e $\{x_{n}\}_n$, $\{y_{n}\}_n$ successioni di Cauchy, mostrare che $\left\{ d(x_n,y_n) \right\}$ è una successione di Cauchy in $\mathbb{R}$.
*Dimostrazione*: Essendo le due successioni di Cauchy esisteranno $\bar{n},\bar{m}\in N$ tali che $\forall n>\bar{n},\exists\varepsilon>0\text{ tale che } |x_n-x_{n+1}|<\varepsilon$, e anche $\forall n>\bar{m},\exists\varepsilon>0\text{ tale che } |y_n-y_{n+1}|<\varepsilon$.
Senza perdita di generalità scelgo $\bar{n}>\bar{m}$, vale che, fissato un $\varepsilon$ che vada bene per entrambe, $d(x_n,y_n)<d(x_n,x_{n+1})+d(y_n,y_{n+1})<2\varepsilon$. Scegliendo $\varepsilon_{1}=\frac{\varepsilon}{2}$ abbiamo che $\left\{ d(x_n,y_n) \right\}$ è di Cauchy.

6. Ogni sottoinsieme di uno spazio indiscreto è compatto.
*Dimostrazione*: Uno spazio topologico $(X,\tau)$ si dice indiscreto se gli unici aperti sono $\varnothing$ e $X$. Sia $A\subset X$, $A$ è diverso da $X$ e non vuoto, quindi è chiuso, l'unica famiglia di aperti possibile è anche finita, ovvero $O=X$, che chiaramente ricopre $A$. Quindi $A$ è compatto.
7. Ogni sottoinsieme di uno spazio con la topologia cofinita è compatto.
*Dimostrazione*: Sia $(X,\tau)$ uno spazio topologico,