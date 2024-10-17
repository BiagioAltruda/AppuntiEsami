Introduzione assiomatica dei *numeri reali*
Esiste un insieme $\mathbb{R}$, munito di due leggi di composizione interna, il $+$ e il $\cdot$ 
$$
+:\mathbb{R}\times \mathbb{R}\to \mathbb{R}
$$
$$
\cdot:\mathbb{R}\times \mathbb{R}\to \mathbb{R}
$$
e di una relazione d'ordine $\leq$, che verificano assiomi algebrici, assiomi di ordinamento e l'assioma di completezza.

**Assiomi Algebrici di $\mathbb{R}$**
1. $\forall a,b \in \mathbb{R}:\,\, a+b=b+a$. (Commutatività della somma)
2. $\forall a,b,c \in \mathbb{R}:\,\, (a+b)+c=a+(b+c)$ (Associatività della somma)
3. $\exists\, 0 \in \mathbb{R},\, \forall a\in \mathbb{R}:\,\, a+0=a$ (Esistenza di un elemento neutro della somma)
4. $\forall a\in \mathbb{R}\,\exists a'\in \mathbb{R}:\,\, a+a'=0$ (Esistenza di un opposto)
5. $\forall a,b \in \mathbb{R}:\,\, a\cdot b=b\cdot a$ (Commutatività del prodotto)
6. $\forall a,b,c\in \mathbb{R}:\,\, (a\cdot b)\cdot c=a\cdot(b\cdot c)$ (Associatività del prodotto)
7. $\exists 1\in \mathbb{R}, 1\neq0 \text{ tale che } \forall a\in \mathbb{R}\,\, a\cdot 1 = a$ (Esistenza di un elemento neutro del prodotto)
8. $\forall a \in \mathbb{R}, \,a \neq 0, \,\, \exists\, a''\in \mathbb{R} \text{ tale che } a\cdot a''=1$ (Esistenza di un reciproco)
9. $\forall a,b,c \in \mathbb{R}:\,\, (a+b)\cdot c= a\cdot c + b\cdot c$ (Proprietà distributiva)

*Osservazioni*:
1. Si dimostra che esiste un unico elemento neutro per il $+$ ed esiste un solo elemento neutro per $\cdot$. Tali elementi si chiamano rispettivamente lo zero di $\mathbb{R}$ e l'unità di $\mathbb{R}$.
	Infatti per l'assioma $3)$ $\exists ù,0 \in \mathbb{R}: \,\, \forall a \in \mathbb{R} a+0 =a$, se $\exists\, 0'\in \mathbb{R}: \,\, \forall a \in \mathbb{R} a+0'=a$, allora avremmo che $0'=0+0'=0$ ovvero $0=0'$. 
	Analogamente per l'assioma $7)$ $\exists 1\in \mathbb{R}, 1\neq 0:\,\, \forall a \in \mathbb{R},\,\, a\cdot 1=a$. Se fosse che $\exists\, 1',\, 1' \neq 0 \text{ tale che }\forall a\in \mathbb{R},\,\, a\cdot 1'=a$, allora $1'=1\cdot 1'=1$. $\blacksquare$ 
	Tale elemento si chiama l'uno di $\mathbb{R}$.
2. Si dimostra che se esiste un opposto di un numero reale, questo è unico. Ovvero per l'assioma $4)$ $\forall a\in \mathbb{R}, \,\, \exists a'\in \mathbb{R}:\,\, a+a'=0$, tale $a'$ è unico e si chiama l'opposto di $a$ e si denota con $-a$. *Dimostrarlo*.
	Analogamente si verifica che esiste, ed è unico, il reciproco di un numero reale, ossia per l'assioma $8)$ $\forall a \in \mathbb{R}, \, a\neq 0, \, \exists\, a'' \text{ tale che } a\cdot a''=1$. Tale $a''$ é unico e si chiama il reciproco di $a$, si denota con $a^{-1}$ oppure $\frac{1}{a}$. *Dimostrarlo*.
3. In matematica si introducono le seguenti notazioni: se $a,b \in \mathbb{R}, \, a-b= a+(-b)$, se $a,b\in \mathbb{R}, \, b\neq 0,\,\, \frac{a}{b} = a\cdot b^{-1}$. 
**Assiomi di ordinamento di $\mathbb{R}$**
$\leq$ é una relazione d'ordine su $\mathbb{R}$ compatibile con la struttura algebrica, ossia $\leq$ verifica i seguenti assiomi di ordinamento:
1. $\forall a\in \mathbb{R}:\,\, a\leq a$ (Riflessibilità)
2. $\forall a,b\in \mathbb{R}, \, a\leq b, b\leq a: \, a=b$ (Antisimmetria)
3. $\forall a,b,c \in \mathbb{R}, \, a\leq b\leq c: \, a\leq c$ (Transitività)
4. $\forall a,b\in \mathbb{R}:\,\, a\leq b \text{ oppure } b\leq a$. (L'ordine è totale)
5. $\forall a,b,c \in \mathbb{R}, a \leq b: \, a+c \leq b+c$ (Compatibilità della $\leq$ con la $+$)
6. $\forall a,b,c \in \mathbb{R},\, a\leq b,\, 0\leq c: \, a\cdot c \leq b \cdot c$ (Compatibilità della $\leq$ con $\cdot$)

*Definizione*:
Gli elementi di $\mathbb{R}$ si chiamano numeri reali.
I numeri reali $a\in \mathbb{R}$ tali che $0\leq a$ si dicono non negativi.
I numeri reali $a\in \mathbb{R}$ tali che $a\leq 0$ si dicono non positivi.
I numeri reali non negativi e diversi da $0$ si dicono positivi.
I numeri reali non positivi e diversi da $0$ si dicono negativi. 

*Notazione*:
Se $a \in \mathbb{R},\, 0 \leq a, \, a\neq 0$ scriveremo $0<a$.
Se $a\in \mathbb{R},\, a\leq 0,\, a\neq 0$ scriveremo $a<0$.

*Proposizione*: 
$\forall a \in \mathbb{R}$ si ha che $a\cdot 0=0$.
*Dimostrazione*:
Sia $a\in \mathbb{R}$. Risulta che $a\cdot 0= a\cdot (0+0)= a\cdot 0 + a\cdot 0$, da cui $a\cdot 0 = a\cdot 0+ a \cdot 0$. Sommo ad entrambi i termini dell'uguaglianza l'opposto di $a\cdot 0$, e quindi:
$$
-a\cdot0 + a\cdot 0= -a\cdot 0 + (a\cdot 0 + a\cdot 0) \implies
$$
$$
0=-a \cdot 0 + a\cdot 0 + a\cdot 0 = 0 + a\cdot 0 = a \cdot 0
$$

*Proprietà* (Legge dell'annullamento del prodotto):
Se $a,b \in \mathbb{R},$ tali che $a\cdot b=0$ allora $a=0$ oppure $b=0$.

*Dimostrazione*
Siano $a,b \in \mathbb{R}$ tali che $a\cdot b = 0$. Supponiamo che $a \neq 0$, allora per l'assioma algebrico $8)$ esiste $a^{-1}\in \mathbb{R},$ tale che $a^{-1}\cdot a=1$. Segue allora che
$$
a\cdot b = 0\implies a^{-1}\cdot(a\cdot b)= a^{-1}\cdot0=0
$$
$$
b=1\cdot b= a^{-1}\cdot(a\cdot b)= a^{-1}\cdot0 
$$
Analogamente se $b \neq 0$ si procede con lo stesso argomento arrivando a $a = 0$. $\blacksquare$

*Osservazione*:
1. Se $a\in \mathbb{R}, a\leq 0$, allora, $-a\leq 0$. Infatti se $0\leq a$, sommando ad entrambi i termini della disequazione per $-a$, risulta che $-a+0\leq -a +a$ ovvero $-a\leq 0$.
2. Se $a,b\in \mathbb{R}, \, a\leq b$, allora $0 \leq b-a$.
3. Se $a,b\in \mathbb{R},\, a\leq b,$ se $c\in \mathbb{R}, \, c\leq0$ allora $b\cdot c \leq a\cdot c$.
4. $\forall a \in \mathbb{R}\, 0 \leq a\cdot a=a^{2}$.
	Segue che $0 \leq 1\cdot 1 = 1$.

*Definizione*:
Siano $A,B \subset \mathbb{R}, \, A\neq \emptyset,\, B\neq \emptyset,$ si dice che $A$ e $B$ sono separati se $\forall a \in A,\, \forall b\in B: \, a\leq b$.

**Assioma di Dedekind** (Assioma di completezza):
$\forall A,B \subset\mathbb{R}, A\neq \emptyset, B\neq \emptyset$, separati, $\exists c\in \mathbb{R}$ tale che $\forall a\in A,\, \forall b\in B:\,\, a\leq c\leq b$.

*Definizione*:
$c$ si dice elemento di separazione tra $A$ e $B$.

*Definizione*:
Se $A,B\subset \mathbb{R}, A\neq 0, B\neq 0$, separati, si dice che $A$ e $B$ sono contigui se esiste un unico elemento di separazione tra $A$ e $B$.

*Definizione*:
$\mathbb{R}$ munito delle leggi di composizione, della somma e del prodotto e della relazione di totale ordine $\leq$, che verificano gli assiomi algebrici, di ordinamento e di completezza si chiama insieme dei numeri reali. 
Si dice che $\mathbb{R}$ è un corpo commutativo totalmente ordinato, completo.

---
*Definizione*:
Sia $x \in \mathbb{R}$. Poniamo 
$$|x|:=\begin{cases}
x \text{ se }0<= x \\ \\
-x \text{ se } x\leq 0
\end{cases}$$
Il numero reale $|x|$ si chiama valore assoluto, o modulo, di $x$.

*Proposizione*:
Per ogni $x,y \in \mathbb{R}$ si ha:
1. $|x|=0 \Leftrightarrow x=0$
2. $0\leq |x|$
3. $|-x|= |x|$
4. $|x|\leq y \Leftrightarrow -y \leq x\leq y$
5. $|x+y| \leq |x|+|y|$ (Disuguaglianza triangolare)
6. $||x|-|y||\leq |x-y|$
7. $|xy|=|x||y|$
8. Se $x\neq 0$, si ha $|x^{-1}|= |x|^{-1}$
*Dimostrazione*: 
$4)$ $x,y\in \mathbb{R}, 0\leq y, \, |x|\leq y$. Se $0\leq x$, si ha che $x\leq y$. E inoltre $-y\leq 0\leq |x|= x\leq y$
Se $x\leq0$, si ha che $-x=|x|\leq y \implies -y\leq x\leq 0\leq y$
Risulta che $-y\leq x\leq y$.
Analogamente si dimostra che se $-y<x<y$ allora $|x|\leq y$.
$5)$ Siano $x,y \in \mathbb{R}$, vogliamo provare che:
$$
|x+y|\leq|x|+|y|
$$
Infatti si ha che $-|x|\leq x\leq |x|$ e anche $-|y|\leq y\leq |y|$.
Sommo termine a termine, ottenendo:
$$
-|x|-|y|\leq x+y \leq |x|+|y|
$$
Ossia
$$
-(|x|+|y|)\leq x+y \leq |x|+|y|
$$
Ma per la proprietà $4)$ si ha che
$$
|x+y|\leq |x|+|y|
$$
$6)$ Siano $x,y \in \mathbb{R}$. Vogliamo provare che
$$
||x|-|y||\leq |x-y|
$$
Infatti si ha che 
$$
|x|=|x-y+y|\leq |x-y|+|y|
$$
da cui
$$
|x|-|y|\leq |x-y|
$$
Inoltre $$
|y|=|y-x+x|\leq |y-x|+|x|
$$
cioè $|y|\leq |x-y|+|x|.$
Da cui
$$
|y|-|x|\leq |x-y| \text{ ossia } -|x-y|\leq |x|-|y|
$$
Segue che 
$$
-|x-y|\leq|x|-|y|\leq |x-y|
$$
Concludendo con
$$
||x|-|y||\leq|x-y|
$$

*Definizione* (Distanza): 
Sia $E$ un insieme non vuoto, Si chiama metrica su $E$ o distanza su $E$ una funzione 
$$d:E\times E\to \mathbb{R}$$
che verifica le seguenti proprietà:
1. $\forall x,y \in E:\,\, 0\leq d(x,y)$
2. $\forall x,y\in E:\,\, d(x,y)=0 \Leftrightarrow x=y$
3. $\forall x,y\in E:\,\, d(x,y)=d(y,x)$
4. $\forall x,y,z \in E: \,\, d(x,z)\leq d(x,y)+d(y,z)$ (Disuguaglianza triangolare)

*Definizione*:
Un insieme $E$ munito di una distanza $d$ si dice spazio metrico

*Proposizione*:
$\forall x,y \in \mathbb{R}:\,\, d(x,y):=|x-y|$.
Allora $d$ è una distanza su $\mathbb{R}$ (la distanza euclidea).

*Dimostrazione*:
Siano $x,y\in \mathbb{R}$. Risulta che $0\leq d(x,y)=|x-y|$.
Se $x,y\in \mathbb{R},\,\, d(x,y)=0 \implies |x-y|=0 \Leftrightarrow x=y$.
Se $x,y \in \mathbb{R},\,\, d(x,y)=|x-y|=|y-x|=d(y,x)$.
Se $x,y,z \in \mathbb{R}:\,\, d(x,z)=|x-z|=|x-y+y-z|\leq |x-y|+|y-z|= d(x,y)+ d(y,z)$. $\blacksquare$

*Definizione*:
La distanza $d(x,y)=|x-y|$ si dice distanza euclidea. L'insieme $\mathbb{R}$ si dice spazio metrico euclideo.

*Osservazione* (Interpretazione geometrica di $\mathbb{R}$):
$\mathbb{R}$ é in corrispondenza biunivoca con la retta euclidea.

*Definizione*:
Sia $A\subset \mathbb{R}$. Diremo che $b\in \mathbb{R}$ è un maggiorante per l'insieme $A$ se:
$$
\forall a\in A:\,\,a\leq b.
$$
Denoteremo con il simbolo $\mathcal{M}_{A}$ l'insieme dei maggioranti per $A$.

*Definizione*:
Sia $A\subset \mathbb{R}$. Diremo che $b\in \mathbb{R}$ è un minorante per $A$ se:
$$
\forall a\in A:\,\, b\leq a.
$$
Denoteremo con il simbolo $\mu_{A}$, l'insieme dei minoranti per $A$

*Definizione*:
Sia $A\subset \mathbb{R}$. Si dice $A$ è limitato superiormente se: $\mathcal{M_{A}}\neq \emptyset$.
Si dice che $A$ è limitato inferiormente se $\mu_{A}\neq \emptyset$.
Si dice che $A$ é limitato se è limitato sia superiormente sia inferiormente.

*Definizione*:
Sia $A\subset \mathbb{R}$. Si dice che $M\in \mathbb{R}$ è un massimo per $A$ se:
$$
M\in A\cap \mathcal{M_{A}},
$$
ossia
$$
\begin{cases}
M\in A \\ \forall a\in A:\,\, a\leq M
\end{cases}
$$

*Definizione*:
Sia $A\subset \mathbb{R}$. Si dice che $m\in \mathbb{R}$ è un minimo per $A$ se:
$$
m\in A\cap\mu_{A},
$$
ossia
$$
\begin{cases}
m\in A \\ \forall a\in A:\,\, m\leq a
\end{cases}
$$

*Proposizione*:
Sia $A\subset \mathbb{R}$ se esiste un massimo per $A$, allora esso è unico.
Se esiste un minimo per $A$, allora esso è unico.
*Dimostrazione*:
Siano $M_{1},M_{2}\in \mathbb{R}$ massimi per $A$. Allora risulta che 
$$
\begin{cases}
M_{1}\in A \\ \forall a\in A:\,\,a\leq M_{1} 
\end{cases}\,\,
\text{ e anche }
\begin{cases}
M_{2}\in A \\ \forall a\in A:\,\,a\leq M_{2} 
\end{cases}
$$
Essendo $M_{1} \in A$, si ha che $M_{1}\leq M_{2}$ ma anche $M_{2}\in A$ quindi $M_{2}\leq M_{1}$. Allora essendo $\leq$ una relazione d'ordine si ha che $M_{1}=M_{2}$. 
Analogamente si mostra l'unicità del minimo. $\blacksquare$

*Notazione*:
Sia $A\subset \mathbb{R}$ e sia $M\in A$ un massimo per $A$, denoteremo $M$ con il simbolo $\max A$.
Se esiste il minimo di $A$, lo denoteremo con $\min A$.

*Proposizione*:
Sia $A\subset \mathbb{R}, \,A\neq \emptyset \text{, e, } B\subset \mathbb{R},\,B\neq \emptyset$. Supponiamo che $A\subset B$ e che esistano il minimo sia di $A$, $\xi_{1}$ e il minimo di $B$, $\xi_{2}$. Allora $\xi_{2}\leq \xi_{1}$.
Inoltre se $\exists \max A=\eta_{1}$ e $\exists \max B=\eta_{2}$, si ha che $\eta_{1}\leq \eta_{2}$.

*Dimostrazione*:
Per ipotesi $\exists \min A =\xi_{1}$ e $\exists \min B = \xi_{2}$, ossia
$$
\xi_{1}\in A \cap \mu_{A} \,\, \xi_{2}\in B \cap \mu_{B}
$$
Vogliamo provare che $\xi_{2}\leq \xi_{1}$.
Poiché $A\subset B$ si ha che
$$
\mu _{B}\subset \mu_{A}.
$$
Segue che, $\xi_{2}\in B\cap\mu B, \text{ ma }\mu_{2}\subset \mu_{}A, \text{ e quindi }\xi_{2}\in\mu_{A}$, ed essendo $\xi_{1}\in A$, allora $\xi_{2}\leq \xi_{1}$.
Analogamente, se esistono il $\max A=\eta_{1}$ ed il $\max B=\eta_{2}$, si prova che $\eta_{1}\leq \eta_{2}\,\, \blacksquare$.

*Teorema* (Teorema di esistenza dell'estremo superiore):
Sia $A\subset \mathbb{R}, \, A\neq \emptyset$. Supponiamo che $\mathcal{M_{A}}\neq \emptyset$. Allora esiste il $\min \mathcal{M_{A}}\in \mathbb{R}$.

*Dimostrazione*:
Per ipotesi $A \neq \emptyset$ e $\mathcal{M_{A}}\neq \emptyset$, tali insiemi $A$ e $\mathcal{M_{A}}$ sono separati, ossia: $\forall a\in A,\, \forall b\in \mathcal{M_{A}}:\,\, a\leq b$. Per l'assioma di completezza di Dedekind:
$$
\exists c\in \mathbb{R} \text{ tale che } \forall a\in A,\, \forall b\in \mathcal{M_{A}}:\,\, a\leq c\leq b.
$$
Proviamo che $c=\min \mathcal{M_{A}}$. Poiché $\forall a\in A,\, a\leq c$ risulta che $c\in \mathcal{M_{A}}$.
Inoltre $\forall b\in \mathcal{M_{A}},\,\, c\leq b$ risulta che $c\in \mu_{\mathcal{M_{A}}}$. 
Segue che $c\in \mathcal{M_{A}}\cap \mu_{\mathcal{M_{A}}}$ da cui $c=\min\mathcal{M_{A}}\,\, \blacksquare$.

*Definizione*:
Sia $A\subset \mathbb{R}, A \neq \emptyset,\, \mathcal{M_{A}}\neq \emptyset$. Si chiama estremo superiore di $A$ il numero reale $\min\mathcal{M_{A}}$, tale numero si denota con il simbolo $\sup A$.
Se $A \neq \emptyset$ e $\mathcal{M_{A}}= \emptyset$ si scrive $\sup A=+\infty$.

Analogamente
*Teorema* (Teorema di esistenza dell'estremo inferiore):
Sia $A\subset \mathbb{R}, \,A \neq \emptyset,$ supponiamo che $\mu_{A}\neq \emptyset$. Allora esiste $\max \mu_{A}\in \mathbb{R}$

*Definizione*: 
Sia $A\subset \mathbb{R}, A \neq \emptyset,\, \mu_{A}\neq \emptyset$. Si chiama estremo inferiore di $A$ il numero reale $\max\mu_{A}$, tale numero si denota con il simbolo $\inf A$.
Se $A \neq \emptyset$ e $\mu_{A}= \emptyset$ si scrive $\inf A=-\infty$.

*Esempio*:
1. 
$A= \left\{ x\in\mathbb{R}:\,\, x\leq1 \right\}$.
$\mathcal{M_{A}}=\left\{ b\in \mathbb{R}|\,\,\forall x \in A: x\leq b \right\}=\left\{  b\in \mathbb{R}\,|\, 1\leq b\right\}$.
$A\cap \mathcal{M_{A}}=\left\{ 1 \right\}=\max A$.

2. 
$B=\left\{ x \in \mathbb{R}\,|\,x<1 \right\}$.
$\mathcal{M_{B}}=\left\{ b\in \mathbb{R}\,|\,b \geq1 \right\}$
$B\cap \mathcal{M_{B}}=\emptyset$. $B$ non ammette massimo.
Per il teorema dell'estremo superiore, il $\sup B=\min \mathcal{M_{B}}$ esiste comunque.
Risulta che $\mu_{\mathcal{M_{B}}}=\left\{ y\in \mathbb{R}\,|\, y\leq 1 \right\}$ da cui segue che $\mathcal{M_{B}}\cap \mathcal{\mu_{\mathcal{M_{B}}}}=\left\{ 1 \right\}= \sup B$.

*Proposizione*:
Sia $A\subset \mathbb{R},\,A\neq \emptyset$. Supponiamo che $\mu_{A}\neq \emptyset$ e $\mathcal{M_{A}}\neq \emptyset$. Allora risulta che $\inf A \leq \sup A$.
Inoltre $\inf A= \sup A \Leftrightarrow A \text{ ha un solo elemento}$.

*Dimostrazione*:
Osserviamo che $\forall a\in A$:
$$
\inf A\leq a\leq \sup A.
$$
da cui $\inf A \leq \sup A$. Inoltre $\inf A = \sup A \Leftrightarrow A=\{a\}, \,a=\inf A=\sup A$.

*Proposizione*:
Siano $A,B \subset \mathbb{R},\,A,B\neq \emptyset$. Supponiamo che esistano $\inf$ e $\sup$ sia di $A$ che di $B$.
Se $A\subset B$, allora
$$
\sup A \leq \sup B
$$
$$
\inf B \leq \inf A
$$
*Dimostrazione*:
Vogliamo dimostrare che $\sup A \leq \sup B$ ossia
$$
\min\mathcal{M_{A}}\leq \min\mathcal{M_{B}}
$$
dato che $A\subset B$, si ha che $\mathcal{M_{B}}\subset \mathcal{M_{A}}$. Applicando la ((proposizione)) riguardante il minimo di insiemi si ha che $\min \mathcal{M_{A}}\leq \min\mathcal{M_{B}}$ e quindi $\sup A \leq \sup B$. Analogo per gli estremi inferiori: $\mathcal{M_{B}} \subset \mathcal{M_{A}}$, applicando la stessa proposizione si ha che $\max\mu_{B}\leq\max\mu_{B}$ cioè $\inf B \leq \inf A$.

*Proposizione*:
Sia $A \subset \mathbb{R}, \, A\neq \emptyset$. Supponiamo che $\exists \max A\in \mathbb{R}$, allora  $\max A= \sup A$.
Analogamente se $\exists \min A \in \mathbb{R}$, allora $\min A=\inf A$.
*Dimostrazione*:
Supponiamo che $\exists \max A=M \in \mathbb{R}$ allora $M \subset A\cap \mathcal{M_{A}}$. Voglio verificare che $M$ è il $\sup A$.
Sia $y\in \mathcal{M_{A}}$. Dato che $M\in A$ si ha che $M\leq y$, segue che $M$ è il più piccolo dei maggioranti di $A\,\blacksquare$.
Analogo per l'estremo inferiore.

**Caratterizzazioni dell'estremo superiore e inferiore**
*Proposizione*:
Sia $A\subset \mathbb{R},\, A\neq \emptyset, \mathcal{M_{A}\neq \emptyset}$,  Sono fatti equivalenti:
1. $\xi=\sup A$
2. $i)$ $\forall a\in A:\, a\leq \xi \in \mathbb{R}$
	$ii)$ $\forall y\in \mathbb{R}, y<\xi:\, \exists a\in A$ tale che $y<a$.

*Dimostrazione*:
Proviamo che $1) \implies 2)$. Per ipotesi $\xi=\sup A\in \mathbb{R}$. Segue che $\xi =\min \mathcal{M_{A}}$ per definizione di estremo superiore, ossia $\xi \in \mathcal{M_{A}}\cap \mu_{\mathcal{M_{A}}}$, ottenendo $\xi \in \mathcal{M_{A}}$. Otteniamo così il punto $i)$
Sia $y \in \mathbb{R}, \,y<\xi$. Essendo $\xi$ il più piccolo dei maggioranti di $A$, si ha che $y \not\in \mathcal{M_{A}}$. Pertanto $\exists a\in A$ tale che $y<a$.
Proviamo che $2) \implies 1)$. Per ipotesi valgono $i)$ e $ii)$. Dalla $i)$ segue che $\xi \in \mathcal{M_{A}}$. Devo verificare che $\xi \in \mu_{\mathcal{M_{A}}}$. Se $y\in \mathcal{M_{A}}$ risulta che $\xi\leq y$. Se fosse $y<\xi$ per la $ii)$ $\exists a\in A:\,\, y<a$ da cui $y\not\in \mathcal{M_{A}}$ che è assurdo.
Segue che $\xi \in \mathcal{M_{A}}\cap \mu_{\mathcal{M_{A}}}$ da cui $\xi=\min\mathcal{M_{A}}=\sup A$

*Proposizione*:
Sia $A\subset \mathbb{R}, A\neq \emptyset, \mu_{A}\neq \emptyset$. Sono fatti equivalenti:
1. $\eta=\inf A$
2. $i)$ $\forall a\in A,\, \eta\leq a, \,\eta \in \mathbb{R}$
	$ii)$ $\forall y\in \mathbb{R}:\,\eta<y: \exists a\in A$ tale che $a<y$.

*Corollario* (della caratterizzazione di $\sup$):
Sia $A\subset \mathbb{R}, \, \mathcal{M_{A}}\neq \emptyset$. Sono fatti equivalenti:
1. $\xi=\sup A$.
2. $i)$ $\forall a\in A: a\leq\xi \in \mathbb{R}$
	$ii)$ $\forall \varepsilon>0,\, \exists a\in A$ tale che $\xi-\varepsilon<a$.
*Dimostrazione*:
Supponiamo vera $1)$ e dimostriamo $2)$. Per la caratterizzazione dell'estremo superiore di $A$ risulta vera la $i)$. Sia $\varepsilon \in \mathbb{R},\, \varepsilon>0$. Poniamo $y= \xi-\varepsilon$. Risulta che $y<\xi$, per la $ii)$ della caratterizzazione dell'estremo superiore $\exists a\in A: y<a$. Da cui segue che $\xi-\varepsilon<a\,\blacksquare$.
Supponiamo vera $2)$ e dimostriamo $1)$. Per la caratterizzazione dell'estremo superiore, basta provare che $\forall y\in \mathbb{R},\, y<\xi, \,\exists a\in A:\, y<a$. Sia allora $y\in \mathbb{R}, \,y<\xi$. Poniamo $\varepsilon:= \xi-y, \,\varepsilon \in \mathbb{R}, \,\varepsilon>0$. Per la $ii)$ si ha che $\exists a\in A$ tale che $\xi-\varepsilon<a$. Concludiamo che $y=\xi-\varepsilon \implies y<a \, \blacksquare$.

*Corollario* (della caratterizzazione di estremo inferiore):
Sia $A\subset \mathbb{R}, \mu_{A}\neq \emptyset$. Sono fatti equivalenti:
1. $\eta=\inf A$.
2. $i)$ $\forall a\in A: \eta\leq a, \,\eta \in \mathbb{R}$
	$ii)$ $\forall \varepsilon >0, \,\exists a\in A$ tale che $a<\eta+\varepsilon$.

*Proposizione* (La dimostrazione è sul Buttazzo): 
Siano $A,B\subset \mathbb{R},\, A,B\neq \emptyset, \, A,B$ separati. Sono fatti equivalenti:
1. $A,B$ sono contigui, cioè $\exists!\, c\in \mathbb{R}$ tale che $\forall a\in A,\, \forall b\in B: a\leq c\leq b$.
2. $\sup A = \inf B$.

*Osservazione*:
$A=\left\{ x \in \mathbb{R}|\, x<1 \right\}$, $B=\left\{ x\in \mathbb{R}|\, x>1 \right\}$.
Vale che $\sup A = \inf B$ e sono contigui.

*Proposizione*:
Siano $X,Y\subset \mathbb{R}, X\neq \emptyset,\, Y\neq \emptyset,\, X,Y$ separati. Sono fatti equivalenti:
1. $X,Y$ sono contigui.
2. $\forall \varepsilon>0,\, \exists x \in X,\, \exists y\in Y$ tali che $y-x<\varepsilon$.

*Dimostrazione*:
dimostriamo che $1) \implies 2)$. Si ha che $\sup X = \inf Y$. Sia $\varepsilon>0$. In corrispondenza di $\frac{\varepsilon}{2}$ per il corollario, $\exists x \in X$ tale che $\sup X - \frac{\varepsilon}{2}<x$. In corrispondenza di $\frac{\varepsilon}{2},\, \exists \in Y$ tale che $y<\inf Y + \frac{\varepsilon}{2}$. Segue che
$$y-x < \inf Y + \frac{\varepsilon}{2}- \sup X+ \frac{\varepsilon}{2}= \inf Y + \frac{\varepsilon}{2}- \inf Y + \frac{\varepsilon}{2} = \varepsilon.$$
Concludiamo che $y-x < \varepsilon$.
Dimostriamo che $2)\implies 1)$. Per ipotesi $\forall \varepsilon>0, \exists x \in X,\, \exists y \in Y$ tale che $y-x<\varepsilon$.
Al fine di dimostrare che $\sup X = \inf Y$ verifichiamo che $\forall \varepsilon>0: \,0\leq\inf Y - \sup X < \varepsilon$. (Posso scegliere $\bar{\varepsilon}= \inf Y - \sup X, \, \bar{\varepsilon}>0: \, 0 \leq \inf Y - \sup X < \bar{\varepsilon}= \inf Y - \sup X$.)
Sia quindi $\varepsilon>0$. Per $2)$, $\exists x \in X, \, \exists y\in Y$ tali che $y-x<\varepsilon$.
Segue che $\inf Y - \sup X \leq y-x<\varepsilon$ da cui $\inf Y - \sup X <\varepsilon \,\blacksquare.$

----------
*Definizione*:
Sia $I\subset \mathbb{R}$. Si dice che $I$ è un intervallo se:
$$
\forall a,b \in I,\, a\leq b, \, a\neq b: \, \left\{z\in \mathbb{R}|\, a<z<b \right\}\subset I 
$$

*Notazione per intervalli di estremi $a,b \in \mathbb{R}$ e di semirette*:
Siano $a,b\in \mathbb{R}, \,a<b$. Denoteremo:
1. $]a,a[=\emptyset$,
2. $[a,a]={a}$
3. $]a,b[= \left\{ z \in \mathbb{R}|\, a<z<b \right\}$ (Intervallo aperto di estremi $a,b$).
4. $[a,b]=\left\{ z\in \mathbb{R}| a\leq z\leq b \right\}$ (Intervallo chiuso di estremi $a,b$).
5. $]a,b]= \left\{ z\in \mathbb{R} \, a\leq z<b \right\}$ (Intervallo aperto a destra di estremi $a,b$).
6. $[a,b[= \left\{ z \in \mathbb{R}|\, a<z\leq b \right\}$ (Intervallo aperto a sinistra di estremi $a,b$).
7. $[a,+\infty[=\left\{ z \in \mathbb{R}|, a\leq z \right\}$ (semiretta destra chiusa di estremo $a$).
8. $],a,\infty[= \left\{ z \in \mathbb{R}|\, a<z \right\}$ (semiretta destra aperta di estremo $a$)
9. $]-\infty,b]= \left\{ z\in \mathbb{R}| z\leq b \right\}$ (semiretta sinistra chiusa di estremo $b$).
10. $]-\infty,b[= \left\{ z\in \mathbb{R}| z< b \right\}$ (semiretta sinistra aperta di estremo $b$).
11. $]-\infty,+\infty[ = \mathbb{R}$

*Teorema* (Caratterizzazione degli intervalli di $\mathbb{R}$):
Sia $I\subset \mathbb{R}$. Sono fatti equivalenti:
1. $I$ è un intervallo.
2. $I$ è un intervallo di estremi reali, oppure $I$ è una semiretta destra, oppure $I$ è una semiretta sinistra, oppure $I=\emptyset$ oppure $I=\mathbb{R}$, oppure $I$ è ridotto ad un solo elemento.

*Dimostrazione*:
$2) \implies 1)$ è ovvia. Dimostriamo $1)\implies2)$. Sia $I\subset \mathbb{R}$ un intervallo. Se $I$ è vuoto o ridotto ad un solo elemento allora vale $2)$. Supponiamo $I$ di non essere in uno di questi casi e che $I$ sia limitato. Poniamo $a=\inf I\in \mathbb{R}$ e $b= \sup I\in \mathbb{R}$. Verifichiamo che
$$
]a,b[\subset I\subset [a,b]
$$ La seconda inclusione è ovvia, dimostriamo la prima.
Sia $y\in ]a,b[$. Allora $\inf I<y<\sup I$. Per le caratterizzazioni di estremo superiore e inferiore di $I$, $\exists x \in I,$ tale che $y<x$, $\exists x' \in I$ tale che $x'<y$.
Pertanto $x,x'\in I, \, y\in \mathbb{R},\,\, x'<y<x$. Essendo $I$ un intervallo si ha che $y \in I$.
Supponiamo poi che $I$ sia limitato solo inferiormente. Risulta che $a= \inf I \in \mathbb{R}, \, \sup I = +\infty$. Si dimostra che $]a,+\infty[\subset I \subset [a,+\infty[$. 
Analogamente se $I$ è limitato solo superiormente.
Se $I$ non è limitato, allora $I=\mathbb{R}\, \blacksquare.$

---------
*Definizione*:
Sia $A\subset \mathbb{R}$. Si dice che $A$ è induttivo se:
1. $0\in A$
2. $x \in A \implies x+1\in A$

*Esempio*:
$A=[0,+\infty[$ è induttivo, dato che $0\in A$ e $\forall x \in A: x+1\in A$, perché se $0\leq x$ allora $0\leq1\leq x+1$ quindi $x+1\in A$.

*Definizione*:
Si dice insieme dei numeri naturali e si denota con il simbolo $\mathbb{N}$, l'intersezione di tutti i sottoinsiemi induttivi di $\mathbb{R}$.

Posto $\mathcal{F}=\left\{ A\subset \mathbb{R}|\, A \text{ induttivo } \right\}$, si ha che $\mathcal{F}\neq \emptyset$.
Per definizione, poniamo $\mathbb{N}=\cap_{A\in \mathcal{F}}A$.
Ogni elemento di $\mathbb{N}$ è detto numero naturale.

*Proposizione*:
$\mathbb{N}$ è induttivo.

*Dimostrazione*:
Verifichiamo che $\mathbb{N}$ è induttivo. 
$\forall A \in \mathcal{F}: 0 \in A$, segue che $0\in \cap_{A\in \mathcal{F}}A=\mathbb{N}$.
Verifichiamo ora che $x \in \mathbb{N} \implies x+1 \in \mathbb{N}$. Quindi sia $n\in \mathbb{N}$. Risulta che $\forall A \in \mathcal{F}:\, n\in A$. Essendo $A$ induttivo $n+1 \in A, \forall A\in \mathcal{F}$. Allora $n+1 \in \cap_{A\in \mathcal{F}}A=\mathbb{N}$.
Pertanto $\mathbb{N}$ è induttivo $\blacksquare.$

*Osservazione*:
Essendo $\mathbb{N}$ induttivo, si ha che $\mathbb{N}\subset [0,+\infty[$.

**Principio d'induzione**
Sia $A\subset \mathbb{N}$, tale che:
1. $0\in A$
2. $\forall n: (n\in A \implies n+1\in A)$.
Allora si ha che $A=\mathbb{N}$.

*Dimostrazione*:
Per ipotesi $A\subset \mathbb{N}$. Inoltre essendo $A$ induttivo, si ha che $A\in \mathcal{F}$, da cui $\mathbb{N}=\cap_{B\in \mathcal{F}}B\subset A$. Allora $A=\mathbb{N}$.

*Definizione*:
Se $n\in \mathbb{N}$ allora $n+1$ si chiama il successivo di $n$.

*Osservazione*:
 Essendo $\mathbb{N}$ induttivo, ogni successivo di un naturale è un numero naturale.

*Proposizione*:
Risulta che:
1. $\forall n,m\in \mathbb{N},\,\, n+m\in \mathbb{N}$.
2. $\forall n,m\in \mathbb{N},\, n\cdot m\in \mathbb{N}$.

*Dimostrazione*:
Dimostriamo $1)$. Verifichiamo che $\forall n,m\in \mathbb{N}:\, n+m\in \mathbb{N}$.
Sia quindi $m\in \mathbb{N}$. Consideriamo l'insieme $A_{m}=\left\{ n\in \mathbb{N}|\,n+m\in \mathbb{N} \right\}$. Proviamo che $A_{m}=\mathbb{N}$.
Dimostriamolo per induzione.
Infatti risulta che $A_{n}\subset \mathbb{N}$. Inoltre $0\in A_{m}$ poiché $0+m=m\in \mathbb{N}$.
Inoltre sia $n\in A_{m}$, ossia $n+m\in \mathbb{N}$. Consideriamo $(n+1)+m= (n+m)+1$. Essendo $n+m\in \mathbb{N}$ e $\mathbb{N}$ induttivo, concludiamo che $(n+1)+m\in \mathbb{N}$ da cui $n+1\in A_{m}$. Quindi $A_{m}$ è induttivo e per il principio di induzione: $A_{m}=\mathbb{N}$.

Dimostriamo $2)$. Verifichiamo che $\forall n,m\in \mathbb{N}:\, n+m\in \mathbb{N}$.
Sia quindi $m\in \mathbb{N}$. Consideriamo l'insieme $B_{m}=\left\{ n\in \mathbb{N}| n\cdot m\in \mathbb{N} \right\}\subset \mathbb{N}$. Vale che $0\in B_{m}$ essendo $m\cdot 0=0\in \mathbb{N}$.
Verifichiamo che $n\in B_{m}\implies n+1\in B_{m}$. Sia quindi $n\in B_{m}$. Valutiamo $(n+1)m= n\cdot m + m$. $n\cdot m\in \mathbb{N}$ ed essendo $m\in \mathbb{N}$ per come dimostrato sopra $n\cdot m +m \in \mathbb{N}$. Quindi $n+1 \in B_{m}$. Quindi $B_{m}$ è induttivo e allora $B_{m}=\mathbb{N}\, \blacksquare\,$.

**Principio di induzione generalizzato**
Sia $A\subset \mathbb{N}$, sia $n_{0}\in \mathbb{N}$. Supponiamo che:
1. $n_{0}\in A$,
2. $\forall n,\, n_{0}\leq n: \, n\in A \implies n+1\in A$.
Allora risulta che $\left\{ n\in \mathbb{N}| n_{0}\leq n \right\}\subset A$.

*Dimostrazione*:
Poniamo $C=\left\{ n\in \mathbb{N}|\, n+n_{0}\in A \right\}$. Proveremo che $C$ è induttivo.
Ovviamente $0\in C$, inoltre se $n\in C:\, n+1\in C$. Dato che se $n\in C,\, n+n_{0}\in A$ da cui $(n+1)+n_{0}=(n+n_{0})+1\in A$. Concludiamo che $C=\mathbb{N}$ da cui segue che $\left\{ n\in \mathbb{N}|\, n_{0}\leq n \right\}\subset A\,\blacksquare.$

*Osservazione*:
Se $A\subset \left\{ n\in \mathbb{N}|\, n\geq n_{0} \right\}$ e verifica le proprietà richieste dal principio di induzione generalizzato allora $A= \left\{ n\in \mathbb{N}|\, n>n_{0} \right\}$.

*Notazione*:
$]a,b[= (a,b)$

*Teorema* (Discretezza di $\mathbb{N}$): $\forall n\in \mathbb{N}:\, (n,n+1)\cap \mathbb{N}=\varnothing$.

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
Segue che $B$ è induttivo e che $B=\mathbb{N}$. Quindi $\mathbb{N}\cap(n+1,n+2)=\varnothing$, quindi $C$ è induttivo e $C=\mathbb{N}$.
Da cui $\mathbb{N}\cap(n,n+1)=\varnothing,\quad\forall n\in \mathbb{N}\,\blacksquare$.

$\mathbb{N}$ si dice discreto, ossia verifica la proprietà $\forall n\in \mathbb{N}:\, \mathbb{N}\cap(n,n+1)=\varnothing$.

*Teorema*:
$\mathbb{N}$ non è limitato superiormente.

*Dimostrazione*:
Vogliamo provare che $\mathcal{M_{\mathbb{N}}}=\emptyset$. Supponiamo per assurdo che $\mathcal{M_{\mathbb{N}}}\neq \emptyset$. Per il teorema di esistenza dell'estremo superiore, $\exists M=\sup\mathbb{N}\in \mathbb{R}$. Segue che $M\in \mathcal{M_{\mathbb{N}}}$, cioè $\forall n\in \mathbb{N}: \, n\leq M$.
Essendo $\mathbb{N}$ induttivo, si ha che $\forall n\in \mathbb{N}: n+1\in \mathbb{N} \implies \forall n\in \mathbb{N}, n+1\leq M$.
Pertanto vale che $\forall n\in \mathbb{N}: n\leq M-1$, ma allora $M-1$ è un maggiorante di $\mathbb{N}$, che è assurdo in quanto avevamo supposto che $\sup\mathbb{N}=M. \, \blacksquare$.

*Proposizione* (Proprietà archimedea di $\mathbb{R}$ (I)):

$\forall a\in \mathbb{R},\, a>0:\, \exists n\in \mathbb{N}$ tale che $a<n$.

*Dimostrazione*:
Per il teorema precedente, si ha che $\mathcal{M_{\mathbb{N}}}=\emptyset$. Voglio dimostrare che $\forall a \in \mathbb{R},\, a>0, \exists n\in \mathbb{N}$ tale che $a<n$. Sia quindi $a \in \mathbb{R}, \,a>0$.
Se per assurdo che la tesi sia falsa, ovvero che $\forall n\in \mathbb{N},\,a\geq n$.
Pertanto si ha che $a\in \mathcal{M_{\mathbb{N}}}$, assurdo $\blacksquare$.

*Proposizione* (Proprietà archimedea II):

$\forall a,b\in \mathbb{R},\, a,b>0,\, \exists n\in \mathbb{N}$ tale che $na>b$. 

*Dimostrazione*:
Sia $a,b\in \mathbb{R}, \,a,b>0,\, a>b,$. Poiché $a\neq 0,\,\exists a^{-1}\in \mathbb{R}$.
Consideriamo il numero reale $x=b\cdot a^{-1}$. Per la proprietà archimedea (I), $\exists n\in \mathbb{N}, \,$ tale che $n>x=b a^{-1}$.
Pertanto essendo $a>0$, risulta che $na> xa=(b a^{-1})a= b \,\blacksquare.$

*Corollario*:
Se $x\in\mathbb{R},\, x\geq 0$, tale che $\forall n\in \mathbb{N}, \, n\neq 0,\, x\leq \frac{1}{n}$, allora $x=0$.

*Dimostrazione*:
Sia $x\geq 0$ tale che $\forall n\in \mathbb{N}, n\neq 0,\, x\leq \frac{1}{n}$.
Se fosse che $x\neq 0$, allora $x>0$. Per la proprietà archimedea (I) applicata a $x^{-1}\in \mathbb{R}$, $\exists \bar{n} \in \mathbb{N},\, \bar{n}\neq 0$, tale che $\bar{n}> x^{-1}$. Segue che $$x> \frac{1}{\bar{n}}.$$
Quindi si ha che $\frac{1}{\bar{n}}< x \leq \frac{1}{\bar{n}}$, allora $\frac{1}{\bar{n}}< \frac{1}{\bar{n}}$, assurdo $\,\blacksquare$.

*Corollario*:
Se $x \in \mathbb{R}, \, x>0$, allora $\exists n\in \mathbb{N},\, n\neq 0$ tale che $x> \frac{1}{n}$.

*Dimostrazione*:
Sia $x \in \mathbb{R},\, x>0$. Per il corollario precedente, se $\forall n\in \mathbb{N},\, n\neq 0, \, x\leq n$ allora $x=0$. Essendo $x> 0$, $\exists n\in \mathbb{N},\, n\neq 0$ tale che $x> \frac{1}{n}\, \blacksquare$.

*Definizione*:
$\mathbb{R}$ si dice un corpo, commutativo, archimedeo completo e totalmente ordinato.

*Proposizione* (Principio del minimo):
Ogni sottoinsieme $A \subset \mathbb{N}, \, A\neq \emptyset$, ammette minimo.

*Dimostrazione*:
Sia $A\subset \mathbb{N},\, A \neq \emptyset$. Risulta che $0\in\mu_{A}\neq \emptyset$. Per il teorema di esistenza dell'estremo inferiore in $\mathbb{R}$, $$
\exists \inf A=\max\mu_{A}=a\in \mathbb{R}.
$$
Proveremo che $a=\min A$, cioè $a\in \mathbb{N}$.
Poiché $0<1$, risulta che $a< a+1$, per la caratterizzazione dell'estremo inferiore, $\exists n\in A$ tale che $a\leq n< a+1$. Se $a=n$, la tesi sarebbe soddisfatta, ossia $\inf A\in \mathbb{N} \implies \inf A = \min A$. Se $a<n<n+1$, allora per la caratterizzazione dell'estremo inferiore $\exists m\in A$ tale che $a\leq m<n$. Segue che $m<n<a+1\leq m+1$ da cui $n\in]m,m+1[$ che è assurdo in quanto $]m,m+1[=\emptyset$. (Discretezza di $\mathbb{N}$). Concludiamo che $a=n$ $\blacksquare.$

*Definizione*:
$\mathbb{N}$ si dice ben ordinato in quanto $\mathbb{N}$ verifica il principio del minimo.

*Definizione*:
Si dice che $n\in \mathbb{N}$ è pari se $n=2p$, con $p \in\mathbb{N}$. Si dice che $n\in \mathbb{N}$ è dispari se $n=2m +1$, con $m\in \mathbb{N}$.
\
Denoteremo con $\mathbb{P}$ l'insieme dei naturali pari e $\mathbb{D}$ l'insieme dei naturali dispari.

*Proposizione*:
1. $\mathbb{P}\cup \mathbb{D}=\mathbb{N}$
2. $\mathbb{P}\cap \mathbb{D}$.

*Dimostrazione*:
1. Verifichiamo che $A=\mathbb{P}\cup \mathbb{D}\subset \mathbb{N}$ soddisfa le ipotesi del principio di induzione.
	Osserviamo che $0\in \mathbb{P}\subset A=\mathbb{P}\cup \mathbb{D}$. Proveremo anche che $A$ è induttivo. Sia $n\in A=\mathbb{P}\cup \mathbb{D}$. Se $n=2p$, con $p \in \mathbb{N}$, allora $n+1=2p+1 \in \mathbb{D}\subset A$. Se invece, $n=2m+1$, con $m\in \mathbb{N}$, allora $n+1=2m+1+1= 2(m+1)$, allora $n+1\in \mathbb{P}\subset A$.
	Segue che $\forall n\in \mathbb{N}, n\in A$, allora $n+1\in A$. Per il principio di induzione $A=\mathbb{P}\cup \mathbb{D}=\mathbb{N}\, \blacksquare.$
2. Vogliamo provare che $\mathbb{P}\cap \mathbb{D}=\emptyset$. Sia per assurdo che $\exists n\in \mathbb{P}\cap \mathbb{D}$. Allora $n=2p$, con $p \in \mathbb{N}$ ma anche $n=2m+1$, con $m\in \mathbb{N}$. Ovvero: $$
2p=2m+1 \implies 2(p-m)=1.
$$
	Se $p=m, 2\cdot 0=0=1$, assurdo.
	Se $p<m$, allora $2(p-m)=1$. Ma $p-m<0$ cioè $1=2(p-m)<0$, assurdo.
	Se $p>m$, allora per la discretezza di $\mathbb{N}$ si ha che $p-m\geq 1$. Risulta allora che $1=2(p-m)\geq 2$, assurdo $\blacksquare$.

*Teorema*:
Ogni sottoinsieme $A\subset \mathbb{N}$, $A\neq \emptyset, \, \mathcal{M_{A}}\neq \emptyset$ ammette massimo.

*Dimostrazione*:
(Analogo al principio del minimo).

**Numeri relativi (interi)**

*Definizione*:
Si dice $x \in \mathbb{R}$ è un numero relativo se $\exists n,m\in \mathbb{N}:\, x=m-n$.
Si denotano con il simbolo $\mathbb{Z}$.

*Proposizione*:
Valgono le seguenti proprietà:
1. $\mathbb{N}\subset \mathbb{Z}$.
2. $\forall x,y\in \mathbb{Z}: x+y \in \mathbb{Z}, x\cdot y\in \mathbb{Z}, -x \in \mathbb{Z}$.

*Dimostrazione*:
1. $m\in \mathbb{N}$, allora $m=m-0\in \mathbb{Z}$.
2. Siano $x,y\in \mathbb{Z}$. Allora per definizione $x=m-n,\,y=p-q$, con $m,n,p,q\in \mathbb{N}$. Quindi $x+y=m-n+p-q= (m+p)-(n+q)\in \mathbb{Z}$. Inoltre siano $x,y$ come prima, $x\cdot y= (m-n)\cdot(p-q)=mp-mq-np+nq=(mp+nq)- (mq+np)\in \mathbb{Z}$. Infine se $x \in \mathbb{Z}, \, x=m-n,\, m,n\in \mathbb{Z}$, allora $-x=-(m-n)=n-m\in \mathbb{Z}$.

*Teorema*:
Sia $A\subset \mathbb{Z}, \, A\neq \emptyset,\, \mu(A)\neq \emptyset$, allora $A$ ammette minimo. 

*Teorema*:
$\mathbb{Z}$ non è limitato superiormente, $\mathbb{Z}$ non è limitato inferiormente.

*Dimostrazione*:
La tesi segue osservando $\mathbb{N}\subset \mathbb{Z}$ e anche $-\mathbb{N}\subset \mathbb{Z}$.

*Teorema*:
Ogni sottoinsieme $A\subset \mathbb{Z},\, A\neq \emptyset, \mathcal{M_{A}}\neq \emptyset$ ammette massimo.


**Numeri razionali**

*Definizione*:
Si dice che $x \in \mathbb{R}$ è un numero razionale se $\exists m\in \mathbb{Z}, n\in \mathbb{N},\, n\neq 0 \text{ tali che } x=m\cdot n^{-1}= \frac{m}{n}$.
L'insieme dei numeri razionali si denota con $\mathbb{Q}$.
Si dice che $x \in \mathbb{R}$ è un numero irrazionale se $x \in \mathbb{R}\setminus \mathbb{Q}$.

*Proposizione*:
Valgono le seguenti proprietà:
1. $\mathbb{Z}\subset \mathbb{Q}$
2. $\forall x,y\in \mathbb{Q},\, x+y\in \mathbb{Q},\, xy\in \mathbb{Q},\, -x \in \mathbb{Q}$
3. $\forall x \in \mathbb{Q}, x\neq 0:\, x^{-1}\in \mathbb{Q}$

*Dimostrazione*:
1. Sia $x \in \mathbb{Z},$ in particolare $x=\frac{x}{1}\in \mathbb{Q}$.
2. Siano $x,y\in \mathbb{Q}$. Per definizione $\exists m\in \mathbb{Z}, n\in \mathbb{Z}, n\neq 0,\,\exists p \in \mathbb{Z}, \,q\in \mathbb{N}, q\neq 0$, tali che $x=mn^{-1},\,y=pq^{-1}$. Segue che $x+y=mn^{-1}+pq^{-1}=\frac{mq+pn}{nq}\in \mathbb{Q}$. Inoltre $xy=(mn^{-1})(pq^{-1})= \frac{m}{n}\cdot \frac{p}{q}=(mp)(nq)^{-1}\in \mathbb{Q}$. Infine si ha che se $x \in \mathbb{Q}$ allora $-x \in \mathbb{Q}$. Infatti se $x=mn^{-1}$, come prima, allora $-x=-m(n^{-1})=(-m)n^{-1}\in \mathbb{Q}$.
3. 


*Teorema*: 
$\mathbb{Q}$ è denso in $\mathbb{R}$. Ovvero: se $a,b\in \mathbb{R}, \,a<b$, allora $\exists q\in \mathbb{Q}$, tale che $a<q<b$.

*Dimostrazione*: Ci sono 3 casi da considerare:
1. Siano $a,b\in \mathbb{R}:\,0\leq a<b$;
	Per l'assioma di Archimede vale che $\exists n\in \mathbb{N}:\, n(b-a)>1 \implies n> \frac{1}{b-a}$,

	Segue che $nb-na>1$, da cui $nb>na+1$.
	Consideriamo l'insieme:
$$
C=\left\{ p \in \mathbb{N}|\, na<p \right\}
$$
	che è non vuoto per la proprietà archimedea. Inoltre $C\subset \mathbb{N}$. Essendo $C\subset \mathbb{N}$, non vuoto, per il principio del minimo $\exists \min C=m\in \mathbb{N}$. Segue che $na<m$, $na+1<nb$, essendo inoltre $m=\min C$, risulta che $m-1 <na$ da cui $m\leq na +1$. Concludiamo che $na<m\leq na+1<nb$ e quindi $na<m<nb$. Moltiplicando per il reciproco di $n$ si ha che $a< mn^{-1}<b$.
	Posto $q=mn^{-1}$, si ha che $q\in \mathbb{Q}$ e $a<q<b$.

2. Siano $a,b\in \mathbb{R}:\,a<0<b$;
Il caso è banale dato che $0\in\mathbb{Q}$.

3. $a<b<0$.
Si procede applicando il punto $1)$ al caso equivalente $0<-b<-a$. Otterremo così $-q$ che è il numero razionale cercato $\blacksquare$.

*Proposizione*:
$\not\exists x \in \mathbb{Q}|\, x^{2}=2$.

*Dimostrazione*:
Supponiamo per assurdo che $\exists x \in \mathbb{Q}| x^{2}=2$. Allora $x=\frac{m}{n}$ con $m\in \mathbb{Z}$ e $n\in \mathbb{N}^{*}$, e senza perdita di generalità sono primi tra di loro.
Essendo $x^{2}=2\implies \frac{m^{2}}{n^{2}}=2$. Cioè $m^{2}=2n^{2}$, segue che $m$ è pari. In particolare il quadrato di un numero pari è pari. Quindi $m^{2}=2n^{2}\implies (2s)^{2}=2n^{2}\implies 4s ^{2}=2n^{2}$. Ovvero $2s^{2}=n^{2}$. Quindi anche $n^{2}$ è pari, e conseguentemente anche $n$. Ma allora sia $m$ che $n$ sono pari che contraddice l'ipotesi di averli scelti coprimi.

*Teorema*(incompletezza di $\mathbb{Q}$):
$\mathbb{Q}$ non verifica l'assioma di Dedekind ($\mathbb{Q}$ non è completo).

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

*Definizione*:
Sia $x \in \mathbb{R}$. Sia $n\in \mathbb{N},\,n \neq0$. Si chiama potenza $n-esima$ di $x$ il numero reale:
$$
x^{n}=\begin{cases}
x^{n} &\text{se } m\in \mathbb{N}^{+}  \\
1 & \text{se } n=0 \\
\frac{1}{x^{|n|}}&\text{se }n\in-\mathbb{N}^{+} 
\end{cases}
$$

*Proposizione*:
$\forall x \in \mathbb{R},\, x\neq 0,\, \forall n,m\in \mathbb{Z}$:
1. $(x^{m})^{n}=x^{mn}$
2. $x^{n+m}=x^{n}\cdot x^{m}$
3. $(x\cdot y)^{n}=x^{n}\cdot y^{n}$.

*Proposizione*:
1. Sia $y\in \mathbb{R},0<y\leq 1$. Si ha che: $\forall n\in \mathbb{N},\,n \neq 0: y^{n}\leq y$.
2. Sia $y\in \mathbb{R},\,y\geq 1$. Si ha che $\forall n\in \mathbb{N},\,n\neq 0: y^{n}\geq y$.

*Dimostrazione*:
1. Sia $y\in \mathbb{R},0<y\leq 1\implies \forall n\in \mathbb{N},\,n\neq 0: y^{n}\leq y$. $P(n)=\forall n\in \mathbb{N}.\,n\neq 0: y^{n}\leq y$, il predicato che dimostreremo per induzione. Proviamo la base induttiva, sia quindi $n=1$. Allora $y^{1}=y$, verificata. Per il passo induttivo assumiamo che se $y^{n}\leq y$, dobbiamo dimostrare: $y^{n+1}\leq y$. Essendo $y^{n+1}=y \cdot y^{n}$ abbiamo che $y\cdot y^{n}\leq y^{2}$, che ci permette di concludere.
2. Sia $y\in \mathbb{R},\,y\geq 1$. $P(n)=\forall n\in \mathbb{N},\,n\neq 0: y^{n}\geq y$. Dimostriamo il predicato per induzione. Il passo base, $P(1)$, è verificato in quanto $y^{1}\geq y$. Dimostriamo il caso $P(n+1)$. Per ipotesi $y^{n}\geq y$. Ma $y^{n+1}=y^{n}y\geq y\cdot y$ per ipotesi. Abbiamo verificato il passo induttivo $\blacksquare$.

*Proposizione*:
Siano $x,y\in \mathbb{R},\, 0<x<y$. Allora $\forall n\in \mathbb{N},\, n \neq 0: x^{n}< y^{n}$.

*Dimostrazione*:
Dimostriamolo per induzione sul predicato $P(n)=\forall n\in \mathbb{N}, n \neq0,\,x<y\implies xy^{n}<y^{n}$.
$P(1)$ è banale in quanto $x^{1}<y^{1}$ per ipotesi. Dimostriamo il caso $P(n+1)$:
$$
x^{n+1}<y^{n+1}\implies x^{n}\leq y^{n}.
$$
Ma $x<y$ per ipotesi e $x^{n}<y^{n}$ per ipotesi induttiva. Quindi $P(n+1)$ è vera $\blacksquare$.

*Teorema*(della radice $n-esima$):
$\forall y\in \mathbb{R}^{*},\,\forall n\in \mathbb{N},\,n\geq 2$, esiste una ed una sola $x\in \mathbb{R}$ positiva tale che $x^{n}=y$.

*Definizione*:
Sia $y\in \mathbb{R}^{*}$, sia $\mathbb{N}\in \mathbb{N},\,n\geq 2$. Si chiama radice $n-esima$ di $y$ l'unica $x$ reale positiva tale che $x^{n}=y$. ($x=\sqrt[n]{ y }$ oppure $x=y^{\frac{1}{n}}$).

*Dimostrazione*(Del teorema):

Fissiamo $y\in \mathbb{R},\, y> 0,\, n\in \mathbb{N},\, n\geq 2$. Proviamo che se $\exists x \in \mathbb{R},\, x>0,$ tale che $x^{n} = y$ allora $x$ è unica. Se per assurdo $x_{1},x_{2}\in \mathbb{R},\, x_{1},x_{2}>0$ e tali che $x_{1}^{n}=y,\,x_{2}^{n}=y$ allora $x_{1}=x_{2}$.
D'altra parte se $x_{1}<x_{2}$ allora si avrebbe che $x_{1}^{n}<x_{2}^{n} \implies y< y$, che è assurdo. Viceversa se $x_{2}<x_{1}$, allora si avrebbe che $x_{2}^{n}<x_{1}^{n} \implies y< y$, che è assurdo.
Quindi se esiste una $x$ come richiesta, è unica.
Per quanto riguarda l'esistenza della radice ennesima, invece, consideriamo l'insieme: $$
A=\left\{ z\in \mathbb{R}|\,z> 0, z^{n}\leq y \right\}.
$$
Proviamo che:
1. $A\neq \emptyset$
2. $A$ è limitato superiormente, ($\mathcal{M_{A}}\neq \emptyset$).
A tal fine distinguiamo due casi: $0<y\leq1$, $y>1$.
Supponiamo che $0<y\leq 1$. Allora si ha che $y^{n}\leq y$. Pertanto $y\in A$, da cui $A\neq \emptyset$. Inoltre si ha che $1\in \mathcal{M_{A}}$. Se fosse che $1\not\in \mathcal{M_{A}}$. Allora $\exists z \in A$ tale che $z>1$, da cui $z^{n}>1$, ma essendo $z\in A,\, 1\geq y\geq z^{n}>1$ che è assurdo.
Se invece, $y>1$. Allora $1^{n}=1<y$, quindi $1\in A$, e quindi $A$ è non vuoto. Inoltre $y\in \mathcal{M_{A}}$, infatti, se $y\not\in A$, $\exists z\in A$ tale che $z>y$. Ma allora $y^{n}<z^{n}$ ma $z^{n}\leq y$ che è assurdo.
Per il teorema di esistenza dell'estremo superiore esiste $x=\sup A\in \mathbb{R}$. Verifichiamo che $x^{n}=y$.
Basta provare che $\forall\varepsilon>0:\,|x^{n}-y|\leq\varepsilon$. Sia quindi $\varepsilon>0$. Poniamo $$\varepsilon'=\min\left(x,\frac{\varepsilon}{2^{n}nx^{n-1}}\right).$$
Proveremo che $(x-\varepsilon')^{n}<x^{n}<(x+\varepsilon')^{n}$. Che segue direttamente dall'osservare che $0\leq x-\varepsilon'<x<x+\varepsilon'$, e dalla proposizione precedente. Verifichiamo inoltre che $(x-\varepsilon')^{n}<y<(x+\varepsilon')^{n}$.
Per provare la disuguaglianza di destra basta osservare che $(x+\varepsilon')^{n}\not\in A$, dato che $x=\sup A$. Segue che $y<(x+\varepsilon')^{n}$.
Per l'altra disuguaglianza, per la caratterizzazione dell'estremo superiore, essendo $x-\varepsilon'<x$, $\exists \bar{x}\in A$, tale che $0<x-\varepsilon'<\bar{x}<x$. Segue che $(x-\varepsilon')^{n}<\bar{x}^{n}\leq y$, perché $\bar{x}\in A$. Pertanto si ha che $(x-\varepsilon')^{n}<y<(x+\varepsilon')^{n}$.
Concludiamo che $$0\leq|x^{n}-y|\leq |(x+\varepsilon')^{n}-(x-\varepsilon')^{n}|=|(x+\varepsilon')-(x-\varepsilon')|\cdot|(x+\varepsilon')^{n-1}+\dots+(x-\varepsilon')^{n-1}|\implies$$
Maggioro i termini misti con $2x$.
$$
|2\varepsilon'|\cdot|(x+\varepsilon')^{n-1}+\dots+(x-\varepsilon')^{n-1}|\leq 2\varepsilon' \cdot (2x)^{n-1}n=2^{n}x^{n-1}n\varepsilon'\leq \frac{\varepsilon}{2^{n}x^{n-1}n}\cdot 2^{n}x^{n-1}n=\varepsilon.
$$
Segue che $0\leq |x^{n}-y|\leq\varepsilon$, e per l'arbitrarietà di $\varepsilon$: $|x^{n}-y|=0 \iff y=x^{n}\, \blacksquare$.

*Osservazione*:
Il teorema appena dimostrato è uno strumento matematico che ci garantisce dati  $y\in \mathbb{R}$ e $n\in \mathbb{N}$, $n\geq2$ l'esistenza e unicità di una soluzione positiva dell'equazione $x^{n}=y$.

*Teorema*(Densità di $\mathbb{R}\setminus \mathbb{Q}$ in $\mathbb{R}$):
Per ogni $a,b\in \mathbb{R}$, con $a<b$, $\exists c\in \mathbb{R}\setminus \mathbb{Q}$ tale che $a<c<b$.

*Dimostrazione*:
Sia $y=2$. Sia $n=2$. Considero, l'equazione $x^{2}=2$. Per il teorema di esistenza e unicità della radice $n-esima$, $\exists! x \in \mathbb{R},\, x> 0$ tale che $x^{2}=2$. Tale $x$ è denotata con $\sqrt{ 2 }$. Inoltre si ha che $z=\sqrt{ 2 }\not\in \mathbb{Q}$. Pertanto $\exists! x \in \mathbb{R}\setminus \mathbb{Q},$ tale che $x^{2}=2$.
Siano $a,b\in \mathbb{R},\, a<b$. Per gli assiomi di $\mathbb{R}$ si ha che $a-\sqrt{ 2 }<b-\sqrt{ 2 }$. Siano $a'=a-\sqrt{ 2 }\in \mathbb{R}$, $b'=b-\sqrt{ 2 }\in \mathbb{R}$, risulta che $a'<b'$. Per il teorema di densità di $\mathbb{Q}$ in $\mathbb{R}$, $\exists q\in \mathbb{Q}$ tale che $a'<q<b'\implies a-\sqrt{ 2 }<q<b-\sqrt{ 2 }$. Concludiamo che $a-\sqrt{ 2 }+\sqrt{ 2 }<q+\sqrt{ 2 }<b-\sqrt{ 2 }+\sqrt{ 2 }\implies a<q+\sqrt{ 2 }<b$. Risulta che $c=q+\sqrt{ 2 }\in \mathbb{R}\setminus \mathbb{Q}$ e $a<c<b$.

*Proposizione*(Proprietà della radice $n-esima$):
1. $\forall y_{1},y_{2}\in \mathbb{R}, 0<y_{1}, 0<y_{2},\, \forall n\in \mathbb{N},\, n\geq 2$ si ha che $\sqrt[n]{ y_{1}y_{2} }=\sqrt[n]{ y_{1} }\sqrt[n]{ y_{2} }.$
	Dimostrazione: Siano $y_{1},y_{2}\in \mathbb{R},\, y_{1},y_{2}>0,\, n\in \mathbb{N},\, n\geq 2$. Per il teorema di esistenza e unicità della radice $n-esima$, $\exists! x_{1}>0,\exists!x_{2}>0$ tali che $x_{1}^{n}=y_{1}$ e $x_{2}^{n}=y_{2}$. Pertanto $(x_{1}x_{2})^{n}=x_{1}^{n}x_{2}^{n}=y_{1}y_{2}$. Segue che $x_{1}x_{2}=\sqrt[n]{ y_{1}y_{2} }$, da cui segue che $\sqrt[n]{ y_{1} }\sqrt[n]{ y_{2} }=\sqrt[n]{ y_{1}y_{2} }$.
2. $\forall y\in \mathbb{R},\, y>0,\, \forall n\in \mathbb{N},\, n\geq 2,\, \forall m\in \mathbb{Z}$: $\sqrt[n]{ y^{m} }=(\sqrt[n]{ y })^{n}$.
3. $\forall y\in \mathbb{R}, y>0,\, \forall h\in \mathbb{N}, h\geq 2,\, \forall k\in \mathbb{N}, k\geq 2$: $\sqrt[h]{ \sqrt[k]{ y } }=\sqrt[hk]{ y }$.
4. $\forall y \in \mathbb{R},\, y> 0, \forall m_{1},m_{2}\in \mathbb{Z},\, \forall n_{1},n_{2}\in \mathbb{N},\, n_{1},n_{2}\neq 0,\, n_{1}\geq2, n_{2}\geq 2$: $\frac{m_{1}}{n_{1}}=\frac{m_{2}}{2}\iff m_{1}n_{2}=m_{2}n_{1}$. Allora $\sqrt[n_{1}]{ y^{m_{1}} }=\sqrt[n_{2}]{ y^{m_{2}} }$.
5. $\forall y \in \mathbb{R},\, y>0,\, \forall n\in \mathbb{N},\, n\geq 2$: $\sqrt[n]{ y^{n} }=y$.
	Dimostrazione: Sia $y\in \mathbb{R},\, y>0$, sia $n\in \mathbb{N},\, n\geq2$. Posto $x=\sqrt[n]{ y^{n} }$, si ha che $x^{n}=y^{n}$. Segue che $x=y$, da cui segue che $\sqrt[n]{ y^{n} }=y$.
6. $\forall y \in \mathbb{R}, \forall n\in \mathbb{N}, n\geq 2$ tali che $y^{n}\geq 0$: $\sqrt[n]{ y^{n} }=|y|$.
7. $\forall y_{1},y_{2}\in \mathbb{R},\, y_{1}>0,y_{2}>0,\, \forall n\in \mathbb{N}, n\geq 2, y_{1}< y_{2}$: $\sqrt[n]{ y_{1} }\leq \sqrt[n]{ y_{2} }$.

*Definizione*(Potenza razionale):
Sia $y\in \mathbb{R},y>0$. Sia $q\in \mathbb{Q},\, q=\frac{m}{n},\,m\in \mathbb{Z},\,n\in \mathbb{N},\, n\neq 0$. Si chiama potenza razionali di $y$ di esponente $q$ il numero reale: $y^{q}=\sqrt[n]{ y^{m} }$.