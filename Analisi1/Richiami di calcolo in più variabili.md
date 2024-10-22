*Definizione* (Differenziabilità e differenziali): 
Sia $U\subseteq \mathbb{R}^{m}$ un aperto e sia $f:U\to \mathbb{R}^{n}$ una funzione. $f$ è *differenziabile* in $x_{0}\in U$ se esiste una funzione lineare $L:\mathbb{R}^{m}\to \mathbb{R}^{n}$ tale che $$
f(x_{0}+v)=f(x_{0})+L(v)+o(|v|)
$$
In tal caso $L$ è unica e si dice *differenziale* di $f$ in $x_{0}$ e si denota $df_{x_{0}}:\mathbb{R}^{m}\to \mathbb{R}^{n}$.

---
Se $f$ è $\mathbb{R}-$lineare allora coincide con il proprio differenziale.

Il differenziale di una composizione è la composizione dei differenziali.

---
*Definizione*(derivate parziali):
Se $\left\{ e_{i} \right\}$ è la base canonica di $\mathbb{R}^{m}$ allora definiamo la $i-$esima derivata parziale di $f$ come $$
df_{x_{0}}(e_{i})=\frac{\partial f}{\partial x_{i}}(x_{0}).
$$
---
*Proposizione*(Proprietà del differenziale):
siano $f_{1},f_{2}:U\to \mathbb{C}\text{ con }U\subseteq \mathbb{R}^{m}$ aperto, mappe differenziabili in $P$, allora:
1. $\left( d \bar{f_{1}} \right)_{P}=\left( \overline{df_{1}} \right)_{P}$
2. $d(f_{1}f_{2})_{P}=(df_{1})_{P}f_{2}(P)+f_{1}(P)(df_{2})_{P}$
3. Se $f_{1}(P)\neq 0$ allora $\frac{1}{f_{1}}$ è definita in un intorno di $P$ e $$
d\left( \frac{1}{f_{1}} \right)_{P}=\frac{(df_{1})_{P}}{f_{1}(P)^2}
$$


[[Funzioni Olomorfe]]

#MultivariableCalculus
