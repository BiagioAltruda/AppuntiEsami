Siano $f,g:X\to Y$ due funzioni continue. Una omotopia tra $f$ e $g$ è una funzione continua $$
H:X\times[0,1]\to Y
$$
tale che:
1. $H(x,0)=f(x)$
2. $H(x,1)=g(x)$
Stiamo così definendo una damiglia di funzioni $H_{t}=H(\cdot,t):X\to Y$ che possiamo interpretare come uno snapshot di una trasformazione continua di $f$ in $g$.
Se esiste una omotopia tra $f$ e $g$ scriviamo $f \simeq g$ e diciamo che $f$ e $g$ sono mappe omotope.
*Proposizione*(l'omotopia è una relazione di equivalenza):
La relazione $f \sim g\Leftrightarrow f \simeq g$ è una relazione di equivalenza sull'insieme delle funzioni continue da $X$ a $Y$.
*Definizione*(inversa omotopica e equivalenza omotopica):
Sia $f:X\to Y$ continua. Una inversa omotopica di $f$ è una mappa $g:Y\to X$ continua tale che $$
g\circ f\simeq id_{X}\qquad f\circ g\simeq id_{Y}
$$
Se $f$ ammette un'inversa omotopica diremo che $f$ è una *equivalenza omotopica* e che $X$ e $Y$ sono omotopicamente equivalenti.

Gli spazi omeomorfi sono omotopicamente equivalenti.
*Proposizione*:
L'equivalenza omotopica è una classe di equivalenza.

*Definizione*(identificazione): 
Una funzione $f:X\to Y$ continua è detta identificazione se valgono le seguenti condizioni:
1. $f$ è surgettiva
2. $A\subset Y$ è aperto se e solo se $f^{-1}(A)$ è aperto (idem per i chiusi)

*Teorema*(identificazione induce omeomorfismo per quoziente):
Siano $f:X\to Y$ una identificazione e $\sim$ una relazione di equivalenza di $X$ data da $x_{1}\sim x_{2}\Leftrightarrow f(x_{1})=f(x_{2})$. Allorra la mappa $\bar{f}:X\diagup\sim\,\to Y$ ottenuta da $f$ passando al quoziente è un omeomorfismo.
#topology 