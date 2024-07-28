---
tags: funzioni
---


Il concetto di infinitesimo si rivela molto importante sia come notazione che per ottenere una migliore comprensione di quale sia la *parte principale* di una funzione. 

Siano $f,g$ due funzioni infinitesime per $x\to x_{*}$, con $g(x)\neq0$ in un intorno di $x_{*}$; si dice che $f(x)$ è infinitesima di ordine superiore a $g(x)$ per $x\to x_{*}$ se 
$$
\lim_{ x \to x_{*} } \frac{f(x)}{g(x)}=0;
$$
in tal caso si scrive $f(x)=o(g(x));x_{*}$, che si legge $f$ è $o$ piccolo di $g$.

---
*Proposizione 6.44*: siano $f_{1}=o(g_{1}),\,\,f_{2}=o(g_{2})$; allora le funzioni
$$
\frac{f_{1}+g_{1}}{f_{2}+g_{2}}\qquad\text{e}\qquad \frac{g_{1}}{g_{2}}
$$
hanno lo stesso comportamento per $x\to x_{*}$.
*Dimostrazione*:
basta osservare che $$
\frac{f_{1}+g_{1}}{f_{2}+g_{2}}=\left( \frac{\frac{f_{1}}{g_{1}}+1}{\frac{f_{2}}{g_{2}}+1} \right) \cdot\frac{g_{1}}{g_{2}}
$$
e che la quantità tra parentesi tende ad $1$ per $x \to x_{*}$.

---
Valgono (anche se con un leggero abuso di notazione) le seguenti proprietà:
siano $f,g$ due funzioni e $k\in \mathbb{R}$ allora
$$
\begin{gather}
k\,o(f)=o(f) \\
o(f)+o(f)=o(f)\\
o(o(f))=o(f)\\
f\cdot o(g)=o(fg)\\
o(f)\cdot o(g)=o(fg)\\
f=o(g) \quad\Rightarrow\quad \frac{o(f)}{g}=o\left( \frac{f}{g} \right)
\end{gather}
$$

#funzioni 