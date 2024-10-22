*Teorema*: $(\mathbb{Q}, \leq)$ non è completo come spazio metrico.
*Dimostrazione*: Basta trovare un insieme limitato, non vuoto, che non ammette estremo superiore (o inferiore) in $\mathbb{Q}$.
Sia quindi $A=\left\{ x \in \mathbb{Q}:\,x\geq 0 ,\,x^{2}<2\right\}$. $1$ appartiene ad $A$, quindi è non vuoto, $2\in \mathcal{M}_{A}$ infatti:
$$
x^{2}<2 \Rightarrow x^{2} < 4 \Rightarrow x^{2}-4<0 \Rightarrow (x-2)(x+2)<0 \Rightarrow x<2.
$$
Quindi $A$ è superiormente limitato. Supponiamo che $\exists \lambda \in \mathbb{Q}:\, \lambda=\sup A$, in particolare vale $\lambda\geq1$.
Ci sono $3$ casi distinti:
$$
1. \,\lambda^{2}<2 \qquad\qquad\qquad 2.\, \lambda^{2}=2 \qquad\qquad\qquad 3.\,\lambda^{2}>2.
$$
1. Per il [[Principio di Archimede|principio di Archimede]] $\exists n\in \mathbb{N}: n>\max \left\{ 1, \frac{2\lambda+1}{2-\lambda^{2}} \right\}$. Vale che $\lambda+ \frac{1}{n}\in \mathbb{Q}$, vediamo se appartiene ad $A$. Sarebbe a dire:
$$
\left( \lambda+ \frac{1}{n} \right)^{2}= \lambda^{2}+ \frac{2\lambda}{n}+ \frac{1}{n^{2}}< \lambda^{2} + \frac{2\lambda}{n}+ \frac{1}{n}= \lambda^{2}+ \frac{2\lambda+1}{n}.
$$
Se fosse minore di $2$ avremmo:
$$
\lambda^{2}+ \frac{2\lambda+1}{n}<2 \Rightarrow \left( \lambda+ \frac{1}{n} \right)^{2} <2 \Rightarrow \left( \lambda+ \frac{1}{n} \right)\in A.
$$
Ma $\lambda$ era l'estremo superiore di $A$. Otteniamo un assurdo.
2. Senza perdita di generalità posso scrivere $\lambda= \frac{m}{n}$ con $m,n\in \mathbb{Q}$ e coprimi. Se fosse che $\lambda^{2}=2$ avrei:
$$
\frac{m^{2}}{n^{2}}=2 \Rightarrow m^{2}=2n^{2}\Rightarrow \exists p \in \mathbb{N}: \, m=2p.
$$
$$
\frac{4p^{2}}{n^{2}}=2\Rightarrow 2p^{2}=n^{2}.
$$
Cioè sia $m$ che $n$ sono pari, ma li avevamo assunti coprimi, abbiamo ottenuto un assurdo.
3. Ancora per il principio di Archimede scriviamo $\exists n\in \mathbb{N}: \, n>\max\left\{ \frac{1}{\lambda},\frac{2\lambda}{\lambda^{2}-2} \right\}$. Vale che $\lambda - \frac{1}{n}\in \mathbb{Q}$.
$$
\left( \lambda- \frac{1}{n} \right)^{2}= \lambda^{2}- \frac{2\lambda}{n}+ \frac{1}{n^{2}}> \lambda^{2}- \frac{2\lambda}{n}> \lambda^{2} -2\lambda \frac{\lambda^{2}-2}{2\lambda}=\lambda^{2}- \lambda^{2}+2= 2  
$$
Dimostriamo adesso che $\lambda- \frac{1}{n}$ è un maggiorante di $A$.
Ricordando che $x \in A$ implica $x\geq 0$ e usando che $\lambda- \frac{1}{n}$ è positivo si ha che per ogni $x \in A$:
$$
\lambda-\frac{1}{n}>x \Leftrightarrow \left( \lambda-\frac{1}{n} \right)^{2}>x^{2}.
$$
che è vero per quanto detto sopra:
$$
\left( \lambda-\frac{1}{n} \right)^{2}>2>x^{2}
$$
Abbiamo quindi dimostrato che $\lambda-\frac{1}{n}$ è un maggiorante di $A$, in contraddizione al fatto che $\lambda=\sup A$.
Concludendo, $\nexists \lambda \in \mathbb{Q}$ tale che $\lambda=\sup A$. $\blacksquare$
