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