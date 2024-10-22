Indicheremo l'insieme dei cammini da $x_{0}$ a $x_{1}$ in $X$ come $$
\Omega(X,x_{0},x_{1})
$$
Se $X$ è chiaro dal contesto, può essere omesso. Se $x_{0}=x_{1}$ potremo scrivere $\Omega(X,x_{0})$, o anche $\Omega(x_{0})$.
Un [[cammino]] tale che $x_{0}=x_{1}$ si dice *laccio* o *loop*.
Un cammino  $\gamma$ è [[omotopo]] alla funzione costante $x\to\gamma(0)$. In particolare cammini con un estremo in comune sono sempre omotopi.
*Definizione*(Omotopia di cammini):
Una omotopia di cammini (o omotopia a estremi fissato) fra $\gamma_{0},\gamma_{1}\in\Omega(X,x_{0},x_{1})$ è un omotopia $H:[0,1]\times[0,1]\to X$ tale che
1. $H(x,0)=\gamma_{0}(x)$ e $H(x,1)=\gamma_{1}(x)$
2. $H(0,t)=x_{0}$ e $H(1,t)=x_{1}$, cioè $H(\cdot,t)\in\Omega(X,x_{0},x_{1})$.

---
*Proposizione*:
Le omotopie di cammini inducono una relazione di equivalenza su $\Omega(X,x_{0},x_{1})$.

Se $\gamma_{1}$ e $\gamma_{2}$ sono omotope a estremi fissati scriviamo $\gamma_{1}\simeq\gamma_{2}$

*Definizione*(Giunzione):
Siano $\gamma_{1},\gamma_{2}:[0,1]\to X$ cammini tali che $\gamma_{1}(1)=\gamma_{2}(0)$. Definiamo la loro giunzione come la mappa $$
\gamma:[0,1]\to X,\qquad\gamma(t)=\begin{cases} \gamma_{1}(2t)\qquad\text{se }t\in[0,\frac{1}{2}] \\
\gamma_{2}(2t-1)\text{ se }t\in[\frac{1}{2},1]

\end{cases}.
$$
La giunzione di due cammini si indica con $\gamma_{1}*\gamma_{2}$.


*Teorema*: Se $\gamma_{1}\simeq\gamma_{1}'$ in $\Omega(x_{0},x_{1})$ e $\gamma_{2}\simeq\gamma_{2}'$ in $\Omega(x_{1},x_{2})$, allora $\gamma_{1}*\gamma_{2}\simeq\gamma_{1}'*\gamma_{2}'$ in $\Omega(x_{0},x_{2})$

*Definizione* (Gruppo fondamentale):
Sia $X$ uno spazio topologico e sia $x_{0}\in X$. Il gruppo fondamentale o primo gruppo di omotopia di $X$ con *punto base* $x_{0}\in X$ e:
$$
\pi_{1}(X,x_{0})=\Omega(X,x_{0},x_{1})\diagup \simeq
$$
cioè l'insieme delle classi di equivalenza di lacci in $X$ passanti per $x_{0}$ per la relazione di omotopia a estremi fissati.
Osserviamo che $\pi_{1}(X,x_{0})$ dipende solo dalla componente connessa per archi che contiene $x_{0}$.
Il gruppo fondamentale è effettivamente un gruppo con l'operazione di giunzione


#topology 