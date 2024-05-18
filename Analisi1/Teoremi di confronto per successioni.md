*Teorema* (di limitatezza):
Sia $a_n\to l\in\mathbb{R}$, e sia $H<l<K$, allora definitivamente $H<a_n<K$, in particolare, ogni successione convergente è limitata. Invece, ogni successione divergente positivamente è limitata inferiormente.
*Dimostrazione*:
Per la prima parte, osserviamo che ogni intervallo $(H,K)$ è un intorno di $l$, quindi per definizione di limite, definitivamente $a_n\in(H,K)$, concludo con la limitatezza.
La seconda parte segue dalla definizione di limite e dalla proposizione sulla limitatezza delle successioni. $\blacksquare$
*Teorema* (di permanenza del segno):
Sia $\lim_{n\to\infty} a_n\neq0$ allora definitivamente $a_n$ ha lo stesso segno del suo limite.
*Proposizione*:
Siano $\{a_n\}_n$ e $\{b_n\}_n$ due successioni tali che definitivamente $$\{a_n\}_n\leq\{b_n\}_n$$
allora se $a_n\to+\infty\Rightarrow b_n\to+\infty$
alternativamente se $b_n\to-\infty\Rightarrow a_n\to-\infty$
*Dimostrazione*:
Fissato $M\in\mathbb{R}$, definitivamente $a_n>M$ e per ipotesi $b_n\geq a_n$ definitivamente vale quindi: $b_n\geq a_n>M$. Abbiamo quindi provato che $b_n\to+\infty$, l'altro caso è analogo. $\blacksquare$
*Teorema* (dei carabinieri):
Siano $\{a_n\}_n$, $\{b_n\}_n$ e $\{c_n\}_n$ successioni di tali che definitivamente $$a_n\leq b_n\leq c_n$$ e che $$a_n\to l,\qquad c_n\to l$$
allora anche la successione $\{b_n\}_n$ ha limite e, in particolare, tende ad $l$.
*Dimostrazione*:
Dimostriamo il caso $l\in\mathbb{R}$, dato che l'altro è dimostrato nella proposizione precedente. Fissato dunque un intorno $(H,K)$ di $l$, abbiamo che $H<l<K$, quindi definitivamente $H< a_n$ e definitivamente $c_n< K$ quindi definitivamente $H<a_n\leq b_n\leq c_n<K$  ovvero $b_n\in(H,K)$. $\blacksquare$  

---
[[Limite]]

#SuccessionieSerie 