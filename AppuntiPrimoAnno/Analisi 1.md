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
|y|=|y-x+y|\leq |y-x|+|x|
$$
cioè $|y|\leq |x-y|+|x|.$
Da cui
$$
|y|-|x|\leq |x,y| \text{ ossia } -|x-y|\leq |x|-|y|
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
