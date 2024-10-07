*Definizione* (Campo o Corpo commutativo):
Sia $\mathbb{F}$ un insieme munito di due operazioni:
$$
+:\mathbb{F}\times \mathbb{F} \to \mathbb{F}
$$
$$
\cdot: \mathbb{F}\times \mathbb{F} \to \mathbb{F}
$$
La terna $(F,+,\cdot)$ si dice campo se valgono le seguenti proprietà:
1. $\forall a,b,c \in \mathbb{F}, \,\, (a+b)+c=a+(b+c)$ e anche $a(b\cdot c)=a(b\cdot c)$.
2. $\forall a,b \in \mathbb{F},\,\, a+b=b+a$ e anche $a\cdot b=b\cdot a$.
3. $\exists\,\,0_{\mathbb{F}}$ e $1_{\mathbb{F}}$ tali che: $\forall a\in \mathbb{F} a+0_{\mathbb{F}}=a$ e $a\cdot 1_{\mathbb{F}}=a$.
4. $\forall a\in \mathbb{F}, \, \exists b\in \mathbb{F}$ tale che $a+b=0_{\mathbb{F}}$ (e l'opposto è unico).
5. $\exists\,\,b \in \mathbb{F}$ tale che $a\cdot b = 1_{\mathbb{F}}$ ($b=a^{-1}= \frac{1}{a}$).
6. $\forall a,b,c \in \mathbb{F},\, a\cdot(b+c)=a\cdot b+a\cdot c$.
*Osservazioni*:
1. l'opposto di $0_{\mathbb{F}}$ è $0_{\mathbb{F}}$ infatti se cerco $b\in \mathbb{F}$ tale che $0_{\mathbb{F}}+b=0_{\mathbb{F}}$ ma quindi $0_{\mathbb{F}}+b=b$ ma allora $b=0_{\mathbb{F}}+b=0_{\mathbb{F}}$.
2. l'inverso di $1_{\mathbb{F}}$ è $1_{\mathbb{F}}$.
3. $-(-a)=a$.
4. $(-a)\cdot b= a\cdot(-b)=-(a\cdot b)$
5. Se $a\neq0, \,\, (a^{-1})^{-1}=a$.
*Esempi*:
1. $\mathbb{R}$ i numeri reali.
2. $\mathbb{Q}=\left\{ \frac{p}{q}\text{ tali che } p,q\in \mathbb{Z} \right\}$ i numeri razionali.
3. $\mathbb{C}=\{a+b \in \mathbb{R} \text{ tali che } a,b\in \mathbb{R}, i^2=-1\}$ i numeri complessi.
	Definiamo somma e prodotto su $\mathbb{C}$:
	$(a+ib)= (c+id)= (a+c)+i(b+d)$.
	$(a+ib)(c+id)= (ac-bd)+i(ad+bc)$
4. Sia $p$ un numero primo, $\mathbb{F_{p}}$ è il campo di $p$ elementi.
	$\mathbb{F_{p}}=\{0,1,2,\dots,p-1,p\}$.
	Notare che $\forall a\in \mathbb{Z},\,\exists m,r \in \mathbb{Z} \text{ tale che } a=mp+r$ (Contiamo *modulo* p).
	$+:\mathbb{F_{p}}\times \mathbb{F_{p}}\to \mathbb{F_{p}}$, $(a+b)$ è il resto della divisione euclidea $\frac{a+b}{p}$.
	$\cdot: \mathbb{F_{p}}\times \mathbb{F_{p}} \to \mathbb{F_{p}}$, $a\cdot b$ è il resto della divisione euclidea $\frac{ab}{p}$.
5. $\mathbb{N}$ e $\mathbb{Z}$ non sono campi.
*Esercizi*:
1. Dimostrare che $\mathbb{F}_{3}$ è un campo.
2. Dimostrare che $\mathbb{F}_{4}$ non è un campo.

**Spazi Vettoriali**
*Definizione*: Sia $\mathbb{F}$ un campo, definiamo $\mathbb{F}^{n}$, con $n\in \mathbb{N}$ tranne $0$, come $$\mathbb{F^{n}}= \left\{\begin{pmatrix} x_{1}\\x_{2}\\.\\.\\.\\ x_{n}\end{pmatrix} \text{ tale che } x_{1},x_{2},\dots,x_{n}\in \mathbb{F}\right\}$$
Definiamo due operazioni:
$$
+:\mathbb{F}^{n} \times \mathbb{F}^{n} \to \mathbb{F}^{n}, \text{ tale che }
$$
$$
\begin{pmatrix} x_{1}\\x_{2}\\.\\.\\.\\ x_{n}\end{pmatrix} + \begin{pmatrix} y_{1}\\y_{2}\\.\\.\\.\\ y_{n}\end{pmatrix}= \begin{pmatrix} x_{1}+y_{1}\\x_{2}+y_{2}\\.\\.\\.\\ x_{n}+y_{n}\end{pmatrix}
$$
$$
\cdot:\mathbb{F} \times \mathbb{F}^{n} \to \mathbb{F}^{n} \text{ tale che }
$$
$$
\lambda \in \mathbb{F}, \,\, \lambda \cdot \begin{pmatrix} x_{1}\\x_{2}\\.\\.\\.\\ x_{n}\end{pmatrix}= \begin{pmatrix} \lambda x_{1}\\\lambda x_{2}\\.\\.\\.\\ \lambda x_{n}\end{pmatrix}
$$

*Definizione*: Sia $\mathbb{F}$ un campo e $V$ un insieme su cui sono definite due operazioni:
$$
+:V\times V\to V \text{ (Somma)}
$$
$$
\cdot:\mathbb{F} \times V \to V \text{ (Prodotto per scalari)}.
$$
La terna $(V,+,\cdot)$ si dice spazio vettoriale sul campo $\mathbb{F}$ se valgono le seguenti proprietà:
1. $\forall\, u,v,w\in V,\, (u+v)+w=u+(v+w)$ (Associatività della somma)
2. $\forall u,w\in V\, u+v=v+u$ (Commutatività della somma)
3. $\exists\, \underline{0}\in V:\, \forall v\in V,\, v+\underline{0}=v$ ed è detto vettore nullo (Elemento neutro della somma)
4. $\forall v\in V,\,\exists\,v'\in V:\, v+v'=\underline{0}$ e si scrive $-v$ (Opposto per la somma)
5. $\forall a,b\in F,\,\forall \underline{v},\, a(b \underline{v})=(ab) \underline{v}$ (Compatibilità di $\cdot$)
6. $\forall\,v\in V\, 1_{\mathbb{F}}\,\underline{v}= \underline{v}$
7. $\forall a\in \mathbb{F},\,\forall u,v\in V:\, a(u+v)=au+av$ (Distributiva $1$)
8. $\forall a,b\in \mathbb{F},\, \forall v\in V:\, (a+b)v=av+bv$. (Distributiva $2$).

*Esempi*:
Sono spazi vettoriali
1. I vettori geometrici
2. $\mathbb{F}^{n}$, infatti:
	Vale l'associativa della somma perché se
	$$
u,v,w\in \mathbb{F}^{n} \implies u= \begin{pmatrix} u_{1} \\ \cdot \\ \cdot \\ \cdot \\ u_{n}\end{pmatrix}, v= \begin{pmatrix} v_{1} \\ \cdot \\ \cdot \\ \cdot \\ v_{n}\end{pmatrix}, w= \begin{pmatrix} W_{1} \\ \cdot \\ \cdot \\ \cdot \\ w_{n}\end{pmatrix}\\ $$ $$
u+(v+w)=\begin{pmatrix} u_{1} \\ \cdot \\ \cdot \\ \cdot \\ u_{n}\end{pmatrix}+\left( \begin{pmatrix} v_{1} \\ \cdot \\ \cdot \\ \cdot \\ v_{n}\end{pmatrix} + \begin{pmatrix} w_{1} \\ \cdot \\ \cdot \\ \cdot \\ w_{n}\end{pmatrix} \right) = \begin{pmatrix} u_{1}+(v_{1}+w_{1}) \\ \cdot \\ \cdot \\ \cdot \\ u_{n}+(v_{n}+w_{n})\end{pmatrix}= \begin{pmatrix} (u_{1}+v_{1})+w_{1} \\ \cdot \\ \cdot \\ \cdot \\ (u_{n}+v_{n})+w_{n}\end{pmatrix}
$$
	$\underline{0}\in \mathbb{F}^{n}= \begin{pmatrix} 0 \\ \cdot \\ \cdot \\ \cdot \\ 0\end{pmatrix}$, infatti: $\begin{pmatrix} 0 \\ \cdot \\ \cdot \\ \cdot \\ 0\end{pmatrix}+\begin{pmatrix} x_{1} \\ \cdot \\ \cdot \\ \cdot \\ x_{n}\end{pmatrix}=\begin{pmatrix} x_{1} \\ \cdot \\ \cdot \\ \cdot \\ x_{n}\end{pmatrix}$ 
	Siano $a\in \mathbb{F},\, u,v\in \mathbb{F}^{n}$ allora
	$$
a(u+v)= a\left( \begin{pmatrix} u_{1} \\ \cdot \\ \cdot \\ \cdot \\ u_{n}\end{pmatrix}+\begin{pmatrix} v_{1} \\ \cdot \\ \cdot \\ \cdot \\ v_{n}\end{pmatrix} \right) =a\left(\begin{pmatrix} u_{1}+v_{1} \\ \cdot \\ \cdot \\ \cdot \\ u_{n}+v_{n}\end{pmatrix}\right)= \begin{pmatrix} a(u_{1}+v_{1}) \\ \cdot \\ \cdot \\ \cdot \\ a(u_{n}+v_{n})\end{pmatrix}=\begin{pmatrix} au_{1}+av_{1} \\ \cdot \\ \cdot \\ \cdot \\ au_{n}+av_{n}\end{pmatrix}= a\begin{pmatrix} u_{1} \\ \cdot \\ \cdot \\ \cdot \\ u_{n}\end{pmatrix}+a\begin{pmatrix} v_{1} \\ \cdot \\ \cdot \\ \cdot \\ v_{n}\end{pmatrix}=au+av
$$

3. Verificare il resto delle proprietà

*Osservazione*:
1. Se $v,w\in V,\, \text{ con } v-w$ indicherò $v+(-w)$.
Valgono le seguenti proprietà:
1. $\forall v\in V,\, 0_{\mathbb{F}}\, v=\underline{0}$
2. $\forall s\in\mathbb{F},\, s\,0_{V}=0_{V}$
3. $\forall v\in V,\, (-1_{\mathbb{F}})v=-v$
4. Siano $s \in \mathbb{F},\, v\in V,\, \text{se }sv=0_{V} \implies s=0 \text{ oppure }v=0_{V}$

*Esercizio*: Dimostrare le proprietà da $1)$ a $4)$

---
Sia $V$ uno spazio vettoriale su $\mathbb{F}$ e $v_{1},\dots,v_{n}\in V$ e $\alpha_{1},\dots,\alpha_{n}\in \mathbb{F}$, posso sommare i vettori e moltiplicarli per $\alpha_{i}$ e quindi

*Definizione*:
Sia $V$ spazio vettoriale su $\mathbb{F}$, siano $v_{1},\dots,v_{n}\in V$ e $\alpha_{1},\dots,\alpha_{n}\in \mathbb{F}$, il vettore $$
\alpha_{1}v_{1}+\alpha_{2}v_{2}+\dots+\alpha_{n}v_{n} =v
$$
$v$ si dice combinazione lineare di $v_{1}\dots,v_{n}$ a coefficienti $\alpha_{1},\dots,\alpha_{n}$.

*Esempio*:
Considero in $\mathbb{R}^{3}$ i vettori: $v_{1}=\begin{pmatrix}1 \\2\\0\end{pmatrix}, v_{2}=\begin{pmatrix}-1\\-1\\-1\end{pmatrix}, v_{3}=\begin{pmatrix} \frac{1}{2}\\0\\1\end{pmatrix}, v_{4}=\begin{pmatrix}0\\0\\-2\end{pmatrix}$
e $\alpha_{1}=-1,\,\alpha_{2}=0,\,\alpha_{3}=4,\,\alpha_{4}=2$, allora:
$$
\alpha_{1}v_{1}+\alpha_{2}v_{2}+\dots+\alpha_{4}v_{4}=-1\begin{pmatrix}
1\\2\\0\end{pmatrix} +0\begin{pmatrix}
-1\\-1\\-1
\end{pmatrix} + 4\begin{pmatrix}
\frac{1}{2}\\0\\1
\end{pmatrix}
+2\begin{pmatrix}
0\\0\\-2
\end{pmatrix}
=\begin{pmatrix}
1\\-2\\0
\end{pmatrix} =v
$$

---
*Definizione*:
Fissato un campo $\mathbb{F}$, una matrice con $m$ righe e $n$ colonne a coefficienti in $\mathbb{F}$ è una tabella $A$
$$
A=\begin{pmatrix}
\alpha_{1}  & \alpha_{12} & \dots & \alpha_{1n}\\
\alpha_{21} & \alpha_{22} & \dots & \alpha_{2n}\\

\dots  & \dots & \dots  & \dots\\
\alpha_{m1}  & \alpha_{m2} & \dots & \alpha_{mn}
\end{pmatrix}
$$
$\forall i=1,\dots,m, \, j=1,\dots,n, \, \alpha_{1j}\in \mathbb{F}$
Oppure si scrive $A=(\alpha_{ij})_{1\leq i\leq m\,\, 1\leq j\leq n}$
Indicheremo con $M_{m,n}(\mathbb{F})$ l'insieme di tutte le matrici $m\times n$ a coefficienti in $\mathbb{F}$.

è possibile definire le seguenti operazioni:
$$+: M_{m,n}(\mathbb{F}) \times M_{m,n}(\mathbb{F})\ \to M_{m,n}(\mathbb{F})$$
$$
\cdot: \mathbb{F} \times M_{m,n}(\mathbb{F}) \to M_{m,n}(\mathbb{F})
$$
Se $A=(a_{ij})$, $B=(b_{ij}) \in M_{m,n}(\mathbb{F})$, se $\lambda \in \mathbb{F}$ allora 
$A+B= (a_{ij}+b_{ij})=\begin{pmatrix} a_{11}+b_{11}  & \dots & a_{1m}+b_{1m}\\\dots&\dots&\dots&\\a_{m1}+b_{m 1} &\dots&a_{mn}+b_{mn}\end{pmatrix}$ 

$$
\lambda A = (\lambda a_{ij}) = \begin{pmatrix}
\lambda a_{11} & \dots& \lambda a_{1m} \\ \dots &\dots&\dots \\ \lambda a_{m1} &\dots& \lambda a_{mn}
\\
\end{pmatrix}
$$

Se $A= \begin{pmatrix} 1 &-7 &0 \\ 2 & 0 & 1\end{pmatrix}$, $B= \begin{pmatrix} 0& 4 & 2\\ 1&1&3\end{pmatrix}$, $\lambda=\frac{1}{3}$

$A+B= \begin{pmatrix}1&-3&2\\ 3&1&2\end{pmatrix}$
$\lambda A=\begin{pmatrix} \frac{1}{3}& -\frac{2}{3} &0 \\ \frac{2}{3} & 0 & -\frac{1}{3}\end{pmatrix}$
*Esercizio*:
Dimostrare che $(M_{m,n}(\mathbb{F}),+,\cdot)$ è uno spazio vettoriale

---
*Esempio*:
Sia $X$ un insieme e $\mathbb{F}$ un campo. Definiamo $\mathbb{F}^X=\left\{ f:X \to \mathbb{F}|\, f \text{ è una funzione} \right\}$.
Definiamo
$$
+:\mathbb{F}^{X}\times \mathbb{F}^{X} \to \mathbb{F}^{X}
$$
$$
\cdot: \mathbb{F}^{X}\times \mathbb{F}^{X} \to \mathbb{F}^{X}
$$
Se $f,g \in \mathbb{F}^{X}, \, \lambda \in \mathbb{F}$ allora $f+g:X\to \mathbb{F}$ tale che $(f+g)(x)=f(x)+g(x)$.
E anche $\lambda f: X\to \mathbb{F}$ tale che $(\lambda f)(x)=\lambda f(x)$.

---
*Esempio*:
Polinomi a coefficienti in $\mathbb{F}$ di incognita $t$.
$\mathbb{F}[t]=\left\{ a_{n}t^{n}+a_{n-1}t^{n-1}+\dots+a_{1}t+a_{0}|\, a_{i}\in \mathbb{F},\, \forall i=1,\dots,n, \, n>0 \right\}$.
$$
+: \mathbb{F}[t]\times \mathbb{F}[t] \to \mathbb{F}[t]
$$
$$
\cdot: \mathbb{F}[t] \times \mathbb{F}[t] \to \mathbb{F}[t]
$$

Se $p,q \in \mathbb{F}[t],\, \lambda \in \mathbb{F}$, $p=a_{n}t^{n}+\dots+a_{0}$, $q=b^{n}t^{n}+\dots+b_{0}$. Allora 
$\lambda \cdot p= \lambda a_{n}t^{n}+\dots+\lambda a_{0}$.
$p+q=(a_{n}+b_{n})t^{n}+\dots+(a_{0}+b_{0})$.
Posso interpretare $p$ e $q$ come funzioni da $\mathbb{R}\to \mathbb{R}$, la somma appena definita coincide con la somma di funzioni, quella definita sopra. E lo stesso per il prodotto per scalari.

*Definizione*:
Se $p=a_{n}t^{n}+\dots+a_{0}\in \mathbb{F}[t]$, si dice grado di $p$, indicato con $deg(p)$, quel numero $n\geq0$  tale che $a_{n}\neq0$ e $a_{j}=0,\, \forall j>n$.

I polinomi si possono anche scrivere come:
$$
p=\sum_{i=1}^{n} a_{i}t^{i}
$$
---
**Sottospazi vettoriali**

*Definizione*:
Sia $V$ uno spazio vettoriale sul campo $\mathbb{F}$. $W\subset V$ si dice sottospazio vettoriale di $V$ se soddisfa:
1. $W\neq \emptyset$
2. $\forall u,v\in W,\,\forall \lambda,\mu \in \mathbb{F}$ si ha che $\lambda u+\mu v\in W$

*Osservazione*:
1. Se $W$ è sottospazio di $V$ allora $W$ è spazio vettoriale sullo stesso campo di $V$
2. Le condizioni $1)$ e $2)$, della definizione di sopra, sono equivalenti alla $2)$ e alla $1')$ cioè $0_{V}\in W$. 
	Infatti se $W\neq \emptyset \implies \exists v\in W\implies \forall\lambda \in \mathbb{F}:\,\lambda v\in W$. Quindi se $\lambda=0_{F} \implies 0v \in W \implies 0_{V}\in W$.
	Viceversa se $0_{V}\in W \implies W\neq \emptyset$.
3. $\left\{ 0_{V} \right\}$ è un sottospazio vettoriale.
4. $V$ è sottospazio vettoriale di $V$.
5. $\left\{ \underline{0} \right\}$ è l'unico sottospazio vettoriale di $V$ con un numero finito di elementi se $\mathbb{F}$ ha infiniti elementi.

*Osservazione:*
Quali sono tutti i sottospazi vettoriali di $\mathbb{R}^{2}$ e $\mathbb{R}^{3}$ ?.
Chiaramente $\mathbb{R}^{n}$ è sottospazio di $\mathbb{R}^{n}$ e $\left\{ \underline{0} \right\}$ è sottospazio.
1. In $\mathbb{R}^{2}$, sia $v\in \mathbb{R}^{2}$ e $v\neq \underline{0}$, se $W$ è un sottospazio e $v\in W$. Allora per $2)$, $\forall \lambda \in \mathbb{R},\, \lambda v\in W$. Cioè $W$ contiene tutta la retta passante per l'origine e $v$.
	Se $W$ contiene $w$ che non è multiplo di $v$, allora $W$ contiene anche tutta la retta tra $\underline{0}$ e $w$. Ma allora ottengo tutto $\mathbb{R}^{2}$, dato che $v$ e $w$ non sono allineati.
	Quindi tutti i sottospazi vettoriali di $\mathbb{R}^{2}$ sono: il vettore nullo, le rette per l'origine ed $\mathbb{R}^{2}$ stesso.
2. In $\mathbb{R}^{3}$ tutti e soli i sottospazi vettoriali sono: il vettore nullo, le rette e i piani passanti per l'origine e tutto $\mathbb{R}^{3}$.

------------

**Numeri complessi**
Nascono come estensione dei numeri reali.

*Osservazione*:
Considero l'equazione $x^{2}+1=0$, e ne cerco le soluzioni reali cioè
$$
\left\{ x \in \mathbb{R}|\, x^{2}+1=0 \right\} =\emptyset
$$
Perché $\forall x \in \mathbb{R},\, \,x^{2}\geq0 \implies x^{2}+1 > 0$
Si introduce allora un nuovo "numero" che chiamiamo $i$, tale che $i^{2}=-1$. $i$ è detto unità immaginaria.

*Definizione*:
Si dice numero complesso ogni scrittura della forma: $a+ib,\,a,b\in \mathbb{R}$. E si definisce l'insieme dei numeri complessi come $\mathbb{C}=\left\{ a+ib|\, a,b\in \mathbb{R} \right\}$

*Definizione*:
$\forall z\in \mathbb{C},\, z=a+ib$, $a$ è detto parte reale, $\mathrm{Re}(z)$, e $b$ è detto parte immaginaria, $\mathrm{Im}(z)$.
Ad esempio se $z=\sqrt{ 3 }-5i$. $\mathrm{Re}(z)=\sqrt{ 3 }$, $\mathrm{Im}(z)=-5$.

Due numeri complessi $z=a+ ib$ e $z'=a'+b'i$ sono uguale se e solo se $a=a'$ e $b=b'$.

*Osservazione*:
Per assegnare un numero complesso $z=a+ib$ diamo una coppia ordinata $(a,b)$ di numeri reali. Perciò possiamo rappresentare il numero complesso $z$ come il punto $(a,b)\in R\times \mathbb{R}=\mathbb{R}^{2}$.
Infatti la funzione  $$f:\mathbb{R}^{2}\to \mathbb{C}\, \text{ tale che } (a,b)\to a+ib$$
*Definizione*:
Su $\mathbb{C}$ sono definite delle operazioni di somma e prodotto.
Siano $z=x+iy$ e $z'=x'+iy'$, due numeri complessi allora:

$$
+:\mathbb{C}\times \mathbb{C}\to \mathbb{C}
$$
$$
(z,z')=(x+iy,x'+iy')\to x+x'+i(y+y')
$$
$$
\cdot:\mathbb{C}\times \mathbb{C}\to \mathbb{C}
$$
$$
(z,z')=(x+iy,x'+iy')\to xx'-yy' + i(x'y+xy')
$$

*Proposizione*:
Proprietà della somma e del prodotto:
1. $\forall z,z' \in \mathbb{C},\, z+z'=z'+z$ (Proprietà commutativa della somma)
2. $\forall z,z',z'' \in \mathbb{C}\, z+(z'+z'')=(z+z')+z''$ (Proprietà associativa della somma)
3. $\forall z\in \mathbb{C}: z+0=z$  (Esistenza dell'elemento neutro della somma)
4. $\forall z\in \mathbb{C}:\,\, z+(-z)=0$ (Esistenza degli opposti)
5. $\forall z,z'\in \mathbb{C}:\,\, z\cdot z'=z'\cdot z$ (Proprietà commutativa del prodotto)
6. $\forall z,z',z''\in \mathbb{C}: z\cdot(z'\cdot z'')=(z\cdot z')\cdot z''$ (Proprietà associativa del prodotto)
7. $\forall z,z',z''\in \mathbb{C}: \,\, z\cdot(z'+z'')=z\cdot z' + z\cdot z''$ (Proprietà distributiva)
8. $\forall z\in \mathbb{C}:\,\, z\cdot1=z$ (Esistenza dell'elemento neutro del prodotto)
9. $\forall z\in \mathbb{C}\setminus\{0\}, \,\exists w\in \mathbb{C}: \,\, z\cdot w=1$

*Dimostrazione*:

7. $$z\cdot(z'+z'')= (x+iy)(x'+iy'+x''+iy'')=(x+iy)=(x'+x''+i(y'+y''))=$$
$$
=x(x'+x'')-y(y'+y'')+i(y(x'+x'')+x(y'+y''))= xx'+x x''- yy'-yy''+i(yx'+yx''+xy'+xy'')=
$$
$$
=x x'-yy' +i(yx'+xy') + x x'' - yy'' + i(yx''+ xy'')=z\cdot z' + z\cdot z''\,\, \blacksquare.
$$
9. Cerco $w\in \mathbb{C}$ tale che $z\cdot w=1$. Pongo $z=x+iy$ e $w=u'+iv'$
$$
(x+iy)(u+iv)=1\implies (x-iy)\,(x+iy)(u+iv)=x-iy
$$
$$
(x^{2} +y^{2})(u+iv) =x-iy \implies u+iv= \frac{x-iy}{x^{2}+y^{2}}\implies w=\frac{x}{x^{2}+y^{2}}-i \frac{y}{x^{2}+y^{2}} \Leftrightarrow (x,y)\neq(0,0) \,\blacksquare.
$$
*Osservazione*:
Dalle proprietà viste $(\mathbb{C},+,\cdot)$ è un campo.

*Definizione*:
Sia $z\in \mathbb{C},\, z=x+iy$, si chiama coniugato di $z$ il numero complesso $\bar{z}=x-iy$.

*Proprietà del coniugio*:
$\forall z,w \in \mathbb{C}$ valgono
1. $\bar{\bar{z}}=z$
2. $\overline{z+w}= \bar{z}+\bar{w}$
3. $\overline{z\cdot w}=\bar{z}\cdot \bar{w}$
4. $z=\bar{z} \Leftrightarrow z\in \mathbb{R}$
	dimostrazione di $4)$: $(\implies)$ Sia $z=x+iy$ tale che $x+iy=x-iy\implies x=x$ e anche $y=-y$ $\Leftrightarrow y=0 \implies z\in \mathbb{R}$
	$(\Leftarrow) z \in \mathbb{R},\, x=x+i 0 \implies \bar{z}= \overline{x+i0}=x-i 0=x=z$

*Definizione*:
Sia $z=x+iy \in \mathbb{C}$ si chiama modulo di $z$ il numero reale, indicato con $|z|=\sqrt{ x^{2}+y^{2} }$.

Valgono le seguenti proprietà:
1. $z\in \mathbb{C},\, |z|\geq0$ e $|z|=0 \Leftrightarrow z=0$
2. $\forall z\in \mathbb{C},\, |\bar{z}|=|z|$
3. $\forall z\in \mathbb{C},\, z\cdot \bar{z}=|z|^{2}$
4. $\forall z,w\in \mathbb{C},\, |z\cdot w|=|z|\cdot|w|$
5. $\forall z\in \mathbb{C}, z\neq 0,\, z^{-1}= \frac{\bar{z}}{|z|^{2}}$
