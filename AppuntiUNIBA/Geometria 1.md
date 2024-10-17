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
Per assegnare un numero complesso $z=a+ib$ diamo una coppia ordinata $(a,b)$ di numeri reali. Perciò possiamo rappresentare il numero complesso $z$ come il punto $(a,b)\in \mathbb{R}\times \mathbb{R}=\mathbb{R}^{2}$.
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

--------

*Esempi sottospazi vettoriali*:
Sia $V=\mathbb{R}^{3},\,W=\left\{ (x,y,z)\in \mathbb{R}^{3}|\,3x-y+z=0 \right\}$. è un sottospazio vettoriale.
Dimostriamolo:
1. $W\neq \emptyset$, infatti $\underline{0}=\begin{pmatrix}0\\0\\0\end{pmatrix}\in W$.
2. Mostriamo adesso che $W$ è chiuso per combinazioni lineari.
	Siano $u= \begin{pmatrix}u_{1}\\u_{2}\\u_{3}\end{pmatrix},\,v=\begin{pmatrix}v_{1}\\v_{2}\\v_{3}\end{pmatrix}\in W$, e siano $\lambda,\mu \in \mathbb{R}$. 
	$3u_{1}-u_{2}+u_{3}=0$ ma anche $3v_{1}-v_{2}+v_{3}=0$. Consideriamo $\lambda u+\mu v$:
	$$
\lambda u+\mu v=\begin{pmatrix}
\lambda u_{1}\\\lambda u_{2}\\\lambda u_{3}
\end{pmatrix} + \begin{pmatrix}
\mu v_{1}\\\mu v_{2}\\\mu v_{3}
\end{pmatrix}= \begin{pmatrix}
\lambda u_{1}+\mu v_{1}\\ \lambda u_{2}+\mu v_{2}\\\lambda u_{3}+\mu v_{3}
\end{pmatrix} \implies
$$
$$
3(\lambda u_{1}+\mu u_{1})-\lambda u_{2}-\mu u_{2}+\lambda v_{3}+\mu u_{3}=
$$
$$
\lambda(3u_{1}-u_{2}+u_{3}) + \mu(3v_{1}-v_{2}+v_{3})= \lambda(0)+\mu(0)=0\, \blacksquare.
$$

*Osservazione*:
Se $\underline{0}\not\in W$ allora, $W$ non è sottospazio vettoriale. 

Sia $V=\mathbb{R}^{4}, W=\left\{ (x_{1},x_{2},x_{3},x_{4})\in \mathbb{R}^{4}|\, 2x_{1}-x_{3}=1 \right\}$. $W\neq \emptyset$, infatti $\begin{pmatrix} \frac{1}{2}\\0\\0\\0 \end{pmatrix}\in W$
Ma non è un sottospazio vettoriale dato che $\underline{0}=\begin{pmatrix}0\\0\\0\\0\\\end{pmatrix}$ non rispetta la condizione di $W$. Alternativamente si può fare il seguente controllo:
Siano $\begin{pmatrix}u_{1}\\u_{2}\\u_{3}\\u_{4}\end{pmatrix},\,v=\begin{pmatrix}v_{1}\\v_{2}\\v_{3}\\v_{4}\end{pmatrix}\in W$, e siano $\lambda,\mu \in \mathbb{R}$. Con gli stessi conti di prima otteniamo:
$$
\lambda (2u_{1}-u_{3})+\mu(2v_{1}-v_{3})=\lambda(1)+\mu(1)=\lambda+\mu \neq 1\, \forall \lambda,\mu \in \mathbb{R}
$$
Allora $W$ non è chiuso per combinazioni lineari, quindi non è un sottospazio vettoriale.

--------

Dire se $U\subset \mathbb{R}^{3}$ è sottospazio.
$$
U=\left\{ \begin{pmatrix}
x\\y\\z\\
\end{pmatrix}\in \mathbb{R}^{3}|\,x^{2}-y+2z=0 \right\}.
$$
1. $U\neq \emptyset$ dato che $\underline{0}\in U$.
2. Siano $u,v\in U$, $\lambda,\mu \in U$, considero $\lambda u+\mu v$.
$$ \lambda u+\mu v=
 \begin{pmatrix}
\lambda u_{1}+\mu v_{1}\\ \lambda u_{2}+\mu v_{2}\\\lambda u_{3}+\mu v_{3}
\end{pmatrix}
$$
$$
(\lambda u_{1}+\mu v_{1})^{2}-(\lambda u_{2}+\mu v_{2})+2(\lambda u_{3}+\mu v_{3}) =
$$
$$
\lambda^{2}u_{1}^{2}+2\lambda \mu u_{1}v_{1}+\mu^{2}v_{1}^{2}-\lambda u_{2}-\mu v_{2}+2\lambda u_{3}+2\mu v_{3}= 
$$
$$
\lambda^{2}u_{1}^{2}+2\lambda \mu u_{1}v_{1}+\mu^{2}v_{1}^{2}+\lambda(-v_{1})^{2}+\mu(-v_{1})^{2}= (\lambda^{2}-\lambda)v_{1}^{2}+2\lambda \mu u_{1}v_{3}+(\mu^{2}+\mu)v_{1}^{2}
$$
Che non fa $0, \,\forall \lambda,\mu \in \mathbb{R}$, ad esempio se $u_{1}=v_{1}=1$ $\lambda=\mu =2$ non funziona.

----------

Sia $V=\mathbb{R}[t],$ e sia $W=\left\{ 2at^{2}+3b |\, a,b\in \mathbb{R} \right\}$.
1. Mi chiedo se $\underline{0}\in W$, cioè $\underline{0}=0+0t+0t^{2}+\dots$ 
	Si, mi basta considerare $a=b=0$ allora $2\cdot0t^{2}+3\cdot0\in W$.
2. Siano $p,q\in W,\, \lambda,\mu \in \mathbb{R}$, allora $p=2a_{1}t^{2}+3b_{1}$, e $q=2a_{2}t^{2}+3b_{2}$, Con $a_{1},a_{2},b_{1},b_{2}\in \mathbb{R}$.
	$$\lambda p+\mu q= \lambda(2a_{1}t^{2}+3b_{1})+\mu(2a_{2}t^{2}+3b_{2})$$
$$
2\lambda a_{1}t^{2}+2\mu a_{2}t^{2}+3\lambda b_{1}+3\mu b_{2}= 2(\lambda a_{1}+\mu a_{2})t^{2}+3(\lambda b_{1}+\mu b_{2}).
$$
Che è della forma che cercavo. Quindi $W$ è un sottospazio vettoriale.

----
*Definizione*:
Un sistema di equazioni della forma: $$
\begin{cases}
a_{11}x_{1}+a_{12}x_{2}+\dots+a_{1n}x_{n}=b_{1} \\
\dots \\
\dots \\
a_{m1}x_{1}+a_{m 2}x_{2}+\dots+a_{mn}x_{n}=b_{m}
\end{cases}
$$
Con $a_{ij}\in \mathbb{F},\, b_{i}\in \mathbb{F},\, i=1,\dots,m,\,j=1,\dots,n$. è detto sistema lineare con $m$ equazioni ed $n$ incognite. Gli $a_{ij}$ si dicono coefficienti del sistema, le $x_{j}$ incognite del sistema e i $b_{i}$ termini noti.
Se $b_{i}=i, \,\forall i$, il sistema è detto sistema lineare omogeneo.

La matrice $A=(a_{ij})\in M_{m,n}(\mathbb{F})$, è detta matrice associata al sistema.
Il vettore $b= \begin{pmatrix}b_{1}\\b_{2}\\.\\.\\b_{m}\end{pmatrix}$ si dice vettore dei termini noti, e $x=\begin{pmatrix}x_{1}\\x_{2}\\.\\.\\x_{n}\end{pmatrix}$ vettore delle incognite.
Si scrive $Ax=b$ per indicare il sistema precedente.
Inoltre indico con $A'=(A|b)$, la matrice ottenuta da $A$ "aggiungendo" la colonna $b$, e si chiama matrice completa associata al sistema.

*Esempi*:
1. $$
\begin{cases}
2x_{1}-3x_{2}+4x_{3}-x_{4}=2  \\
-x_{1}+x_{2}+\frac{1}{2}x_{4}=\pi
\end{cases}
$$
$$
A=\begin{pmatrix}
2 &-3&4&-1\\ -1&1 & 0 & \frac{1}{2}
\end{pmatrix}
$$
$b=\begin{pmatrix}2 \\\pi\end{pmatrix}$
$$
A'=\begin{pmatrix}
2&-3&4&-1 &2 \\ -1&1&0& \frac{1}{2} & \pi
\end{pmatrix}
$$
2. $$
\begin{cases}
2x_{1}-x_{2}=0  \\
x_{1}+x_{2}=0 \\
3x_{1}=0
\end{cases}
$$
è un sistema omogeneo
$A=\begin{pmatrix}2 &1 \\1&1\\3&0\end{pmatrix}$, $b=\underline{0}$, $A'=\begin{pmatrix} 2&1&0\\1&1&0\\3&0&0\end{pmatrix}$.
3. $$
\begin{cases}
3x=2
\end{cases}
$$
$A=(3)$, $A'=(3|2)$.

*Teorema*:
Sia $W\subset \mathbb{F}^{n}$, l'insieme delle soluzioni del sistema lineare omogeneo $Ax=\underline{0}$, con $A\in M_{m,n}(\mathbb{F})$ e $\underline{0}\in \mathbb{F}^{n}$.
$W=Sol(Ax=\underline{0})$. Allora $W$ è sottospazio vettoriale di $\mathbb{F}^{n}$.

*Dimostrazione*:
Devo dimostrare che $\underline{0}\in \mathbb{F}^{n}$ appartiene a $W$ e che $\forall z,t\in W,\,\forall\alpha,\beta \in \mathbb{F},\, \alpha z+\beta t\in W$.
$\underline{0}\in W$, infatti: $\underline{0}=\begin{pmatrix}0\\0\\.\\.\\0\end{pmatrix}\in \mathbb{F}^{n}$,
$$Ax=\underline{0}: \begin{cases}
a_{11}x_{1}+\dots+1_{1n}x_{n}=0 \\
. \\
. \\
a_{m1}x_{1}+\dots+a_{mn}x_{n}=0
\end{cases}$$

Ogni sistema lineare omogeneo ammetta la soluzione nulla.

Siano ora $z=\begin{pmatrix}z_{1}\\.\\.\\z_{n}\end{pmatrix}$ e $t=\begin{pmatrix}t_{1}\\.\\.\\t_{n}\end{pmatrix}\in W$, allora $z_{1},\dots,z_{n}$ e $t_{1},\dots,t_{n}$ sono soluzioni del sistema di sopra. Cioè $\forall i=1,\dots,m$, $a_{i 1}z_{1}+\dots+a_{in}z_{n}=0$ e $a_{i 1}t_{1}+\dots+ a_{in}t_{n}=0$.

 Allora considero $\alpha z+\beta t=\begin{pmatrix}\alpha z_{1}+\beta t_{1}\\.\\.\\\alpha z_{n}+\beta t_{n}\end{pmatrix}$, è vero che questo nuovo vettore soddisfa tutte le equazioni del sistema?
 Sia $i\in\{1,..,n\}$, allora $a_{i1}x_{1}+\dots+a_{in}x_{n}=0$, sostituisco il vettore di sopra:
 $$
a_{i 1}(\alpha z_{1}+\beta t_{1})+\dots+ a_{in}(\alpha z_{n}+\beta t_{n})=
\alpha(a_{i 1}z_{1}+\dots+ a_{in}z_{n})+ \beta(a_{i 1}t_{1}+\dots+a_{in}t_{n})
$$
Ma $a_{i 1}z_{1}+\dots+ a_{in}z_{n}=0$ così come $a_{i 1}t_{1}+\dots+a_{in}t_{n}=0$
$$
\implies \alpha(0)+\beta(0)=0
$$
Allora $\alpha z+\beta t\in W\,\blacksquare.$

*Osservazione*:
In particolare se $z\in Sol(Ax=\underline{0})\implies \forall\lambda \in \mathbb{F}:\, \lambda z\in Sol(Ax=\underline{0})$.

*Esercizio*:
Sia $Ax=b, b\neq\underline{0}$ un sistema lineare. Dimostrare che $Sol(Ax=b)$ non è un sottospazio vettoriale.

*Definizione*:
Sia $V$ uno spazio vettoriale su $\mathbb{F}$, e siano $v_{1},v_{2},\dots,v_{k}\in V$. Definiamo l'insieme $Span(v_{1},\dots,v_{k})$ oppure $<v_{1},\dots,v_{k}>=\left\{ v\in V|\, \exists \alpha_{1},\dots,\alpha_{k}\in \mathbb{F}: v=\alpha_{1}v_{1}+\dots+\alpha_{k}v_{k}\right\}$. Viene detto spazio generato dai vettori $v_{1},\dots,v_{k}$ o insieme delle combinazioni lineari di $v_{1},\dots,v_{k}$.

*Osservazione*:
Se almeno uno tra $v_{1},\dots,v_{k}$ non è il vettore nullo, allora $Span(v_{1},\dots,v_{k})$ ha infiniti elementi.

Un altro modo per scrivere $Span(v_{1},\dots,v_{n})=\left\{  \alpha_{1}v_{1}+\dots+\alpha_{k}v_{k}|\, \alpha_{i}\in \mathbb{F} \right\}$.
E $Span(v)=\left\{ \alpha v|\,\alpha \in \mathbb{F} \right\}$.

*Teorema*:
Sia $V$ spazio vettoriale su $\mathbb{F}$, $v_{1},\dots,v_{k}\in V$. Allora valgono le seguenti proprietà:
1. $\forall i=1,\dots,k,\, v_{i}\in Span(v_1,\dots,v_{k})$.
2. $Span(v_{1},\dots,v_{k})$ è sottospazio vettoriale.
3. Se $W$ è sottospazio di $V$ e $v_{1},\dots,v_{k}\in W$ allora $Span(v_{1},\dots,v_{k})\subset W$
	Oppure anche: $Span(v_{1},\dots,v_{k})$ è il più piccolo sottospazio vettoriale di $V$ che contiene $v_{1},\dots,v_{k}$.
*Dimostrazione*:
1. Dobbiamo mostrare che $\forall i=1,\dots,k, \, v_{1},\dots,v_{k}$. Mi chiedo se $\exists \alpha_{1},\dots,\alpha_{k}\in \mathbb{F}: \,v_{1}=\alpha v_{1}+\dots,\alpha_{k}v_{k}$. Si, infatti, $v_{1}=1v_{1}+0v_{2}+\dots+0v_{n}$. ovvero $\forall i=1,\dots,k,\, v_{i}=0v_{1}+\dots+0v_{i-1}+1v_{i}+0v_{i+1}+\dots+0v_{k}$. Cioè basta prendere $\alpha_{i}=1$ e $\alpha_{j}=0,\,\forall j=1,\dots,k,\, j\neq i$. Allora, in particolare, $Span(v_{1},\dots,v_{k})\neq \emptyset$.
2. Essendo $Span(v_{1},\dots,v_{k})\neq \emptyset$, basta dimostrare che $\forall u,w\in Span(v_{1},\dots,v_{k}),\, \forall \lambda,\mu \in \mathbb{F}:\, \lambda u+\mu w\in Span(v_{1},\dots,v_{k})$. 
	Dato che $u,w \in Span(v_{1},\dots,v_{k})$: $\exists \alpha_{1},\dots,\alpha_{k},$ e $\beta_{1},\dots,\beta_{k}\in \mathbb{F}$ tali che $u=\alpha_{1}v_{1}+\dots+\alpha_kv_{k}$ e $w=\beta_{1}v_{1}+\dots,\beta_{k}v_{k}$.
	Considero $\lambda u+\mu w \implies \lambda(\alpha_{1}v_{1}+,\dots,\alpha_{k}v_{k})+\mu(\beta_{1}v_{1}+\dots,\beta_{k}v_{k})=(\lambda\alpha_{1}+\mu\beta_{1})v_{1}+\dots+(\lambda\alpha_{k}+\mu\beta _{k})v_{k}$, che è una combinazione lineare di $v_{1},\dots,v_{k}$.
3. Sia $w\in Span(v_{1},\dots,v_{k})$. Allora $\exists \gamma_{1},\gamma_{k}\in \mathbb{F}$ tali che $w=\gamma_{1}v_{1}+\dots+\gamma_{k}v_{k}$. Ma $W$ è sottospazio vettoriale di $V$ e contiene $v_{1},\dots,v_{k}$. Ma allora $\forall x_{1},\dots,x_{k}\in \mathbb{F},\, x_{1}v_{1}+\dots+x_{k}v_{k}\in W\implies w\in W \,\blacksquare$.

-------
*Esempi*:
In $\mathbb{R}^{3}$
$v_{1}=\begin{pmatrix}1\\-2\\4\end{pmatrix}, v_{2}=\begin{pmatrix}0\\3\\1\end{pmatrix}$. $Span(v_{1},v_{2})=\left\{\alpha_{1}v_{1}+\alpha_{2}v_{2}|\, \alpha_{1},\alpha_{2}\in \mathbb{R}\right\}=\left\{ \alpha_{1}\begin{pmatrix}1\\-2\\4\end{pmatrix}+\alpha_{2}\begin{pmatrix}0\\3\\1\end{pmatrix}|\, \alpha_{1},\alpha_{2}\in \mathbb{R} \right\}=$
$$
=\left\{ \begin{pmatrix}
\alpha_{1}\\-2\alpha_{1}+3\alpha_{2}\\ 4\alpha_{1}+\alpha_{2}
\end{pmatrix}|\, \alpha_{1},\alpha_{2}\in \mathbb{R} \right\} 
$$

In $M_{2,3}(\mathbb{R})$
$A_{1}=\begin{pmatrix}1 &1&1 \\0&1&0\end{pmatrix}$, $A_{2}=\begin{pmatrix}0&0&0\\2&1&0\end{pmatrix}, \,A_{3}=\begin{pmatrix}0&0&0\\0&0&1\end{pmatrix}$
$$
Span(A_{1},A_{2},A_{3})=\left\{ \gamma_{1}A_{1}+\gamma_{2}A_{2}+\gamma_{3}A_{3}| \gamma_{1},\gamma_{2},\gamma_{3}\in \mathbb{R} \right\} =
$$
$$
=\left\{ \begin{pmatrix}
\gamma_{1}& \gamma_{1} & \gamma_{1}\\ \gamma_{2} & \gamma_{1} + \gamma_{2} & \gamma_{3}
\end{pmatrix} |\gamma_{1},\gamma_{2},\gamma_{3}\in \mathbb{R}\right\} 
$$

*Lemma*:
$\forall n\geq 0$, l'insieme $\mathbb{F}[t;n]=\left\{ a_{n}t^{n}+\dots+a_{0}| a_{0},\dots,a_{n}\in \mathbb{F} \right\}$, i polinomi di grado al massimo $n$ è un sottospazio vettoriale di $\mathbb{F}[t]$. 

*Dimostrazione*:
Infatti $\mathbb{F}[t;n]=Span(t^{n},t^{n-1},\dots,t,1)\,\blacksquare$.

*Esempio*:
In $\mathbb{R}[t,5]$. Considero $p_{1}(t)=t^{5}-3t^{4}+2t$, $p_{2}(t)=2t^{3}+2$, $p_{3}(t)=t^{4}+t^{2}$.
$$Span(p_{1}(t),p_{2}(t),p_{3}(t))=\left\{ \beta_{1}p_{1}(t)+ \beta_{2}p_{2}(t)+\beta_{3}p_{3}(t) |\, \beta_{1},\beta_{2},\beta_{3}\in \mathbb{R}\right\}=$$
$$
=\left\{ \beta_{1}(t^{5}-3t^{4}+2t)+\beta_{2}(2t^{3}+2)+\beta_{3}(t^{4}+t^{2})| \beta_{1},\beta_{2},\beta_{3}\in \mathbb{R} \right\} =$$$$=\left\{ \beta_{1}t^{5}+(-3\beta_{1}+\beta_{3})t^{4}+2\beta_{2}t^{3}+\beta_{3}t^{2}+2\beta_{1}t+2\beta_{2}|\, \beta_{1},\beta_{2},\beta_{3}\in \mathbb{R} \right\}.
$$
**Basi**

*Definizione*:
Sia $V$ spazio vettoriale sul campo $\mathbb{F}$. I vettori $v_{1},\dots,v_{k}\in V$ si dicono linearmente indipendenti se $\forall \alpha,\dots\alpha_{k}\in \mathbb{F},$ tali che $\alpha_{1}v_{1}+\dots+\alpha_{k}v_{k}=\underline{0}\implies \alpha_{1}=\alpha_{2}=\dots=\alpha_{k}=0$.
Viceversa si dicono linearmente dipendenti se $\exists \alpha_{1},\dots,\alpha_{k}\in \mathbb{F}$, non tutti nulli, tali che $\alpha_{1}v_{1}+\dots+\alpha_{k}v_{k}=\underline{0}$.

*Osservazione*:
$v_{1},\dots,v_{k}$ sono linearmente indipendenti se l'unica soluzione dell'equazione:
$$
\alpha_{1} v_{1}+\dots+\alpha_{k}v_{k}=\underline{0}
$$
nelle incognite $\alpha_{i}$, l'unica soluzione è quella nulla ($\alpha_{1}=\dots=\alpha_{k}$).

*Esempio*:
In $\mathbb{R}^{4}$
Sia $v_{1}=\begin{pmatrix}1\\0\\2\\3\end{pmatrix},v_{2}=\begin{pmatrix}0\\-1\\0\\-1\end{pmatrix},v_{3}=\begin{pmatrix}1\\-1\\2\\2\end{pmatrix}$.
Mi chiedo se sono indipendenti.
$$
\alpha_{1}v_{1}+\alpha_{2}v_{2}+\alpha_{3}v_{3}=\underline{0}
$$
$$
\implies \alpha_{1}\begin{pmatrix}
1\\0\\2\\3
\end{pmatrix} + \alpha_{2}\begin{pmatrix}
0\\-1\\0\\-1
\end{pmatrix} + \alpha_{3}\begin{pmatrix}
1\\-1\\2\\2
\end{pmatrix} = \underline{0} \implies \begin{pmatrix}
\alpha_{1}+\alpha_{3} \\-\alpha_{2}-\alpha_{3}\\2\alpha_{1}+2\alpha_{3}\\3\alpha_{1}-\alpha_{2}+2\alpha_{3}
\end{pmatrix}= \begin{pmatrix}
0\\0\\0\\0
\end{pmatrix}
$$
Allora, vedendola come un sistema lineare otteniamo:
$$
\begin{cases}
\alpha_{1}=-\alpha_{3} \\
\alpha_{2}=-\alpha_{3} \\
2(-\alpha_{3})+2\alpha_{3}=0 \\
3(-\alpha_{3})-(-\alpha_{3})+2\alpha_{3}=0
\end{cases}
$$
$\forall \alpha_{3}\in \mathbb{R}$ la terna: $\begin{pmatrix}-\alpha_{3}\\-\alpha_{3}\\-\alpha_{3}\end{pmatrix}$ è una soluzione del sistema.
Infatti $v_{3}=v_{1}+v_{2}$.


In $\mathbb{R}^{3}$
$w_{1}=\begin{pmatrix}1\\1\\0\end{pmatrix},w_{2}=\begin{pmatrix}1\\0\\1\end{pmatrix},w_{3}=\begin{pmatrix}0\\0\\1\end{pmatrix}$.
$\alpha_{1}w_{1}+\alpha_{2}w_{2}+\alpha_{3}w_{3}=\underline{0}$ Allora:
$$
\begin{cases}
\alpha_{1}+\alpha_{2} =0\\
\alpha_{1}+\alpha_{3} =0\\
\alpha_{2}+\alpha_{3}=0
\end{cases}
\implies
\begin{cases}
\alpha_{2}=-\alpha_{1} \\
\alpha_{3}=-\alpha_{1} \\
-\alpha_{1}-\alpha_{1}=0 \implies \alpha_{1}=0
\end{cases} \implies
\begin{cases}
\alpha_{1}=0 \\
\alpha_{2}=0 \\
\alpha_{3}=0
\end{cases}
$$
Allora sono linearmente indipendenti.

*Proposizione*:
Sia $Ax=\underline{0}$, un sistema lineare, omogeneo, con $A\in M_{m,n}(\mathbb{F})$. Il sistema $Ax=\underline{0}$ ha un unica soluzione $x=\underline{0}\Leftrightarrow$ le colonne di $A$, $A_{1},\dots,A_{n}$ sono linearmente indipendenti.

*Dimostrazione*:
Infatti il sistema $Ax=\underline{0}$, lo posso scrivere come:
$$
A_{1}x_{1}+\dots+A_{n}x_{n}=\underline{0}
$$
Quest'equazione ha come soluzione, o solo quella nulla con $x=\underline{0}$ e allora le colonne di $A$ sono indipendenti oppure ne esiste una non nulla, $z\neq\underline{0}$ tale che $A_{1}z_{1}+\dots+A_{n}z_{n}=0$. Allora le colonne di $A$ sono linearmente dipendenti.

*Proposizione*:
Valgono le seguenti proprietà:
1. Sia $v\in V$ allora $v$ è indipendente $\Leftrightarrow\, v\neq \underline{0}$.
2. Se fra i vettori $v_{1},\dots,v_{k}$, c'è il vettore nullo. Allora $v_{1},\dots,v_{k}$ sono linearmente dipendenti.
3. Se $\exists i,j, \,i\neq j$, tali che $v_{i}=v_{j}$. Allora i vettore $v_{1},\dots,v_{k}$ sono dipendenti.

*Proposizione*:
Sia $V$ spazio vettoriale su $\mathbb{F}$ e $v_{1},\dots,v_{k}\in V$. $v_{1},\dots,v_{k}$ sono linearmente dipendenti se e solo se: $\exists i=1,\dots, k$, tale che $v_{i}$ è combinazione lineare degli altri.

*Dimostrazione*:
$(\Rightarrow)$ Per ipotesi $v_{1},\dots,v_{k}$ sono dipendenti. Allora $\exists \alpha_{1},\dots,\alpha_{k}$ non tutti nulli, ad esempio $\alpha _i\neq 0$, tali che $\alpha_{1}v_{1}+\dots+\alpha_{k}v_{k}=0$. Se e solo se $$\alpha_{i}v_{i}=-(\alpha_{1}v_{1}+\dots+\alpha_{i-1}v_{i-1}+\alpha_{i+1}v_{i+1}+\dots+\alpha_{k}v_{k}) \implies$$
$$
v_{i}=-\left( \frac{-\alpha_{1}}{\alpha i} \right)v_{1}+\dots+\left(\frac{-\alpha_{k}}{\alpha_{i}}\right)v_{k}
$$
$(\Leftarrow)$ Per ipotesi$v_{i}=\beta_{1}v_{1}+\dots+\beta_{i-1}v_{i-1}+\beta_{i+1}v_{i+1}+\dots+\beta_{k}v_{k}$. Che è vero se e solo se:
$$
\beta_{1}v_{1}+\dots+\beta_{i-1}v_{i-1}+(-1)v_{i}+\beta_{i+1}v_{i+1}+\dots+\beta_{k}v_{k}=\underline{0}\,\blacksquare.
$$

*Esempio*:

Siano $v_{1}=\begin{pmatrix}1\\0\\2\\3\end{pmatrix},v_{2}=\begin{pmatrix}0\\-1\\0\\-1\end{pmatrix},v_{3}=\begin{pmatrix}1\\-1\\2\\2\end{pmatrix}$.
$v_{3}=v_{1}+v_{2}\implies v_{1}+v_{2}-v_{3}=\underline{0}$.

*Proposizione*:
Sia $V$ spazio vettoriale su $\mathbb{F}$. $v_{1},\dots,v_{k}\in V$ tali che $\exists\alpha_{1},\dots,\alpha_{k-1}$: $v_{k}=\alpha_{1}v_{1}+\dots+\alpha_{k-1}v_{k-1}$. Allora $Span(v_{1},\dots,v_{k})=Span(v_{1},\dots,v_{k-1})$.

*Dimostrazione*:
L'inclusione verso sinistra è ovvia, perché se $v\in Span(v_{1},\dots,v_{k-1})$ allora $\exists \gamma_{1},\dots,\gamma_{k-1}\in \mathbb{F}$ tali che $v=\gamma_{1}v_{1}+\dots+\gamma_{k-1}v_{k-1}=\gamma_{1}v_{1}+\dots+\gamma_{k-1}v_{k-1}+0v_{k}\in Span(v_{1},\dots,v_{k})$.
Per l'altra inclusione invece, sia $w\in Span()v_{1},\dots,v_{k}\implies \exists \delta_{1},\dots,\delta_{k}$ tali che $w=\delta_{1}v_{1}+\dots+\delta_{k}v_{k}$. Essendo $v_{k}$ combinazione lineare degli altri, otteniamo:
$$
w=\delta_{1}v_{1}+\dots+\delta_{k}(\alpha_{1}v_{1}+\dots+\alpha_{k-1}v_{k-1}).
$$
$$
w=(\delta_{1}+\delta_{k}\alpha_{1})v_{1}+\dots+(\delta _{k-1}\alpha_{k-1})v_{k-1}\in Span(v_{1},\dots,v_{k-1}) \, \blacksquare.
$$

*Definizione*:
Sia $V$ spazio vettoriale su $\mathbb{F}$, $v_{1},\dots,v_{k}\in V$, si dicono generatori di $V$ se 
$\forall v\in V,\, \exists\alpha_{1},\dots,\alpha_{k}\in \mathbb{F}$ tali che $v=\alpha_{1}v_{1}+\dots+\alpha_{k}v_{k}$. Ovvero $V=Span(v_{1},\dots,v_{k})$.

*Definizione*:
Sia $V$ uno spazio vettoriale su $\mathbb{F}$, $\mathcal{B}=(v_{1},\dots,v_{n})$ si dice base di $V$ se:
1. $v_{1},\dots,v_{n}$ sono linearmente indipendenti
2. $v_{1},\dots,v_{n}$ sono generatori di $V$.

*Teorema*(Caratterizzazione delle basi):
Sia $V$ spazio vettoriale su un campo $\mathbb{F}$. Sono fatti equivalenti:
1. $\mathcal{B}=(v_{1},\dots,v_{n})$ è una base
2. $v_{1},\dots,v_{n}$ sono tali che $\forall v\in V,\, \exists!\,\alpha_{1},\dots,\alpha_{n}\in \mathbb{F}$ tali che $v=\alpha_{1}v_{1}+\dots+\alpha_{n}v_{n}.$

*Dimostrazione*:
$1)\implies 2)$. Sia $\mathcal{B}$ una base di $V$. Devo dimostrare che $\forall v\in V,$ $\exists!\,\alpha_{1},\dots,\alpha_{n}\in \mathbb{F}$ tali che $v=\alpha_{1}v_{1}+\dots+\alpha_{n}v_{n}$. L'esistenza di $\alpha_{1},\dots,\alpha_{n}$ è garantita dal fatto che $v_{1},\dots,v_{n}$ sono generatori. Resta da dimostrare l'unicità. Per assurdo $\exists v\in V$ tale che $v=\alpha_{1}v_{1}+\dots,\alpha_{n}v_{n}=\beta_{1}v_{1}+\dots+\beta_{n}v_{n}$. Se e solo se $\alpha v_{1}+\dots+\alpha_{n}v_{n}-(\beta_{1}v_{1}+\dots+\beta_{n}v_{n})=\underline{0}$. Allora $(\alpha_{1}-\beta_{1})v_{1}+\dots+(\alpha_{n}-\beta_{n})v_{n}=\underline{0}$. Essendo $\mathcal{B}$ base, $v_{1},\dots,v_{n}$ sono linearmente indipendenti, l'unica combinazione lineare che da il vettore nullo è quella tale che $\alpha_{1}=\beta_{1},\dots,\alpha_{n}=\beta_{n}$. Che dimostra l'unicità.
$2)\implies 1)$. I vettori $v_{1},\dots,v_{n}$ sono generatori perché $\forall v\in V,\, \exists \alpha_{1},\dots,\alpha_{n}\in \mathbb{F}$ tali che $v=\alpha_{1} v_{1}+\dots+\alpha_{n}v_{n}$, per ipotesi. Dimostriamo che sono linearmente indipendenti.
Imponiamo che $\alpha_{1}v_{1}+\dots+\alpha_{n}v_{n}=\underline{0}$. Ma so che $\underline{0}=0v_{1}+\dots+0v_{n}$, però per ipotesi ho unicità della combinazione lineare. Allora $\alpha_{1}=\dots=\alpha_{n}=0\,\blacksquare.$

*Esempi*:
1. 
In $\mathbb{F}^{n}$ è definita la base canonica. $\mathcal{B}(e_{1},\dots,e_{n})$. $e_{1}=\begin{pmatrix}1\\0\\.\\.\\0\end{pmatrix},e_{2}=\begin{pmatrix}0\\1\\0\\.\\0\end{pmatrix},\dots, e_{n}=\begin{pmatrix}0\\0\\.\\.\\1\end{pmatrix}$.
2. 
Sia $d\in \mathbb{N}$. $\mathbb{F}_{d}[t]=\left\{ a_{d}t^{d}+\dots+a_{1}t+a_{0} |\, a_{i}\in \mathbb{F}\right\}$. Allora $\mathcal{B}=(t^{d},t^{d-1},\dots,t,1)$ è una base.

*Definizione*:
Sia $V$ spazio vettoriale sul campo $\mathbb{F}$. $\mathcal{B}=(v_{1},\dots,v_{n})$ una base di $V$. Allora dato $v\in V$definiamo coordinate di $v$ rispetto alla base $\mathcal{B}$, indicato con $F_{\mathcal{B}}(v)=\begin{pmatrix}\alpha_{1}\\.\\.\\\alpha_{n}\end{pmatrix}\in \mathbb{F}^{n}$, tali che $v=\alpha_{1} v_{1}+\dots+\alpha_{_{n}}v_{n}$.

*Osservazione*:
Se cambio base le coordinate cambiano. Se $\mathcal{B}=(v_{1},v_{2},\dots,v_{n})$ è base, $\mathcal{B'}=(v_{2},v_{1},\dots,v_{n})$ è una base diversa. Infatti se $F_{\mathcal{B}}(v)=\begin{pmatrix}\alpha_{1}\\\alpha_{2}\\.\\\alpha_{n}\end{pmatrix} \neq F_{\mathcal{B'}}(v)=\begin{pmatrix}\alpha_{2}\\\alpha_{1}\\.\\\alpha_{n}\end{pmatrix}$.

*Esempi*:
In $\mathbb{F}^{n}$, $\mathcal{B}=(e_{1},\dots,e_{n})$. Sia $v\in \mathbb{F}^{n},\, v=\begin{pmatrix}x_{1}\\x_{2}\\.\\x_{n}\end{pmatrix}, x_{i}\in \mathbb{F}$.
$F_{\mathcal{B}}(v)=\begin{pmatrix}x_{1}\\.\\.\\x_{n}\end{pmatrix}=v$.

*Definizione*:
Sia $V$ spazio vettoriale sul campo $\mathbb{F}$. Sia $\mathcal{A}\subset V$, $\mathcal{B}\subset \mathcal{A}$ si dice sottoinsieme massimale di vettori indipendenti in $\mathcal{A}$ se gli elementi di $\mathcal{B}$ sono indipendenti e se $\forall v\in \mathcal{A},\, \mathcal{B}\cup \left\{ v \right\}$ non sono più indipendenti.


*Proposizione*:
Sia $V$ spazio vettoriale sul campo $\mathbb{F}$. Sia $\mathcal{B}=\left\{ v_{1},\dots,v_{n} \right\}$ base di $V$. Allora $\mathcal{B}$ è un insieme massimale di vettori linearmente indipendenti in $V$.

*Dimostrazione*:
Essendo $\mathcal{B}$ base di $V$, tutti i suoi vettori sono indipendenti. Ora sia $v\in V$. $\mathcal{B}$ è base di $V$ quindi $\exists \alpha_{1},\dots,\alpha_{n}\in \mathbb{F}$ tali che $v=\alpha_{1}v_{1}+\dots+\alpha_{n}v_{n}$. Allora $\left\{ v_{1},\dots,v_{n, v} \right\}$ è formato da vettori dipendenti $\blacksquare$.

*Lemma*:
Sia $\mathcal{B}\subset V$ insieme finito. Se $Span(\mathcal{B})$ contiene un sistema di generatori per $V$ allora $Span(\mathcal{B})=V$.

*Dimostrazione*:
Sia $\mathcal{A}\subset Span(\mathcal{B})$ un insieme di generatori per $V$. Ovvero, $\forall v\in V$ $v$ è combinazione lineare di elementi di $\mathcal{A}$.
$\mathcal{A}\subset Span(\mathcal{B})\implies Span(\mathcal{A})\subset Span(\mathcal{B})\subset V\,\blacksquare$.

*Teorema*:
Sia $\mathcal{A}=\left( v_{1},\dots,v_{n} \right)$ sistema di generatori di $V$ e $\mathcal{B}\subset \mathcal{A}$ sottoinsieme massimale di vettori indipendenti in $\mathcal{A}$. Allora $\mathcal{B}$ è base.

*Dimostrazione*:
Per ipotesi gli elementi di $\mathcal{B}$ sono indipendenti. Devo dimostrare che gli elementi di $\mathcal{B}$ generano $V$. Vorremmo mostrare che $\mathcal{A}\subset Span(\mathcal{B})$, e concludere per il lemma precedente. Per ipotesi $\forall v\in \mathcal{A},\, \mathcal{B}\cup \left\{ v \right\}$ non è linearmente indipendente. Allora ogni elemento di $\mathcal{A}$ lo posso scrivere come combinazione degli elementi di $\mathcal{B}$, quindi $\mathcal{A}\subset Span(\mathcal{B})$. Per il lemma precedente, ho concluso $\blacksquare$.

*Corollario*:
Sia $V$ spazio vettoriale finitamente generato, cioè contenente un sistema finito di generatori. Allora $V$ ammette una base.

*Osservazione*:
Esisto spazi vettoriali che non sono finitamente generati, ad esempio $\mathbb{R}[t]$: i polinomi a coefficienti reali nell'incognita $t$ di grado arbitrario.

*Teorema*(Di completamento):
Sia $V$ uno spazio vettoriale sul campo $\mathbb{F}$. $\mathcal{B}=(v_{1},\dots,v_{n})$ base di $V$, e $w_{1},\dots,w_{p}$ vettori linearmente indipendenti in $V$, con $p\leq n$. Allora $\exists \#n-p$ vettori di $\mathcal{B}$ che uniti a $w_{1},\dots,w_{p}$ formano una base.

*Dimostrazione*:
Per induzione su $p$. Caso $p=1$, sia $w_{1}$ è indipendente cioè $w_{1}$ è non nullo. Essendo $\mathcal{B}$ una base, $\exists! \alpha_{1},\dots,\alpha_{n}\in \mathbb{F}$ tali che $w_{1}=\alpha_{1}v_{1}+\dots+\alpha_{n}v_{n}$. Poiché $w_{1}\neq \underline{0}$, allora gli $\alpha_{i}$ non sono tutti nulli. A meno di riordinare, suppongo che $\alpha_{1}\neq 0$. Ma allora $v_{1}=\frac{1}{\alpha_{1}}\left( w_{1}-\sum_{i=2}^{n}\alpha_{i}v_{i} \right)\in Span(w_{1},v_{2},\dots,v_{n})$ e quindi sono generatori.
Basta dimostrare che sono indipendenti. Siano $\beta_{1},\dots,\beta_{n}\in \mathbb{F}$ tali che $$\beta_{1}w_{1}+\beta_{2}v_{2}+\dots+\beta_{n}v_{n}=\underline{0}\implies \beta_{1}(\alpha_{1}v_{1}+\dots+\alpha_{n}v_{n})+\beta_{2}v_{2}+\dots+\beta_{n}v_{n}.$$
$$
\beta_{1}\alpha_{1}v_{1}+\sum_{i=2}^{n}(\beta_{1}\alpha_{i}+\beta_{i})v_{i}=\underline{0} 
$$
che è una combinazione lineare dei $v_{i}$ che sono indipendenti perché sono una base. Quindi $\beta_{1}\alpha_{1}=0$ ma essendo $\alpha_{1}\neq 0\implies \beta_{1}=0$. Allora $\beta_{i}=0,\, \forall i$.
Supponiamo che il teorema sia vero per $p-1$ vettori e dimostriamolo per $p$ vettori.
$w_{1},\dots,w_{p-1}$ sono indipendenti per ipotesi. Allora, a meno di riordinare, posso supporre che $(w_{1},\dots,w_{p-1},v_{p},\dots,v_{n})$ sono base di $V$. Allora $w_{p}$ è combinazione lineare di $(w_{1},\dots,w_{p-1}.v_{p},\dots,v_{n})$ cioè $\exists! \alpha_{1},\dots,\alpha_{n}\in \mathbb{F}$ tali che $w_{p}=\sum_{i=2}^{p-1}\alpha_{i}w_{i}+\sum_{j=i}^{n}\alpha_{j}v_{j}$. $w_{p}$ non è il vettore nullo, allora gli $\alpha_{i},\alpha_{j}$ non sono tutti nulli. più precisamente almeno uno tra gli $\alpha_{j}$ è diverso da $0$, altrimenti $w_{p}=\sum_{i=1}^{p-1}\alpha_{i}w_{i}$ contro l'indipendenza dei $w_{i}$. A meno di riordinare suppongo che $\alpha_{p}\neq 0$. Allora $$v_{p}=\frac{1}{\alpha_{p}}\left( \sum_{i=1}^{p-1}\alpha_{i}w_{i}+w_{p}-\sum_{j=p}^{n}\alpha_{j}v_{j} \right).$$
Ma allora $v_{p}\in Span(w_{1},\dots,w_{p},v_{p-1},\dots,v_{n})$. Quindi $(w_{1},\dots,w_{p},v_{p+1},\dots,v_{n})$ generano. Basta dimostrare che sono linearmente indipendenti. Infatti $$\sum_{i=1}^{p}\beta_{i}w_{i}+\sum_{i=p+1}^{n}\beta_{j}v_{j}=\underline{0} \implies$$
$$
\implies\sum_{i=1}^{p-1} \beta_{i}w_{i}+\beta_{p}\left( \sum_{i=1}^{p-1} \alpha_{i}w_{i} +\sum_{j=p}^{n}\alpha_{j}v_{j}  \right) +\sum_{j=p+1}^{n}\beta_{j}v_{j}=\underline{0} 
$$
Ma quindi:
$$
(\beta_{1}+\beta_{p}\alpha_{1})w_{1}+(\beta_{2}+\beta_{p}\alpha_{2})w_{2}+\dots+(\beta_{p-1}+\beta_{p}\alpha_{p-1})w_{p-1}+(\beta_{p}\alpha_{p})v_{p}+(\beta_{p}\alpha_{p+1}+\beta_{p+1})v_{p+1}+\dots$$$$\dots+(\beta_{p}\alpha_{n}+\beta_{n})v_{n}=\underline{0}.
$$
Tutti i coefficienti di questa combinazione devono essere nulli, ma in particolare lo è $\beta_{p}\alpha_{p}$, ma $\alpha_{p}\neq 0$, quindi $\beta_{p}=0 \implies \beta_{i}=0,\, \forall i\,\blacksquare$.

*Corollario*:
Sia $V$ spazio vettoriale sul campo $\mathbb{F}$. $\mathcal{B},\mathcal{B'}$ basi. Allora $\mathcal{B}$ e $\mathcal{B'}$ hanno lo stesso numero di elementi.
