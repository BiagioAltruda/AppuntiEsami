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
