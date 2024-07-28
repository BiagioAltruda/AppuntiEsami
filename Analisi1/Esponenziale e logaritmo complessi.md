*Definizione*:
Definiamo l'esponenziale complesso come $$
e^{z}=\sum_{n=0}^{\infty} \frac{z^{n}}{n!}.
$$
Ha raggio di convergenza infinito. in particolare converge sempre assolutamente.

*Proposizione*(Proprietà dell'esponenziale complesso):
Valgono i seguenti fatti:
1. $e^{z+w}=e^{z}e^{w}$ per ogni $z,w\in \mathbb{C}$. In particolare $(e^{z})^{-1}=e^{-z}$ quindi $exp:\mathbb{C}\to \mathbb{C}^{\times}$ è ben definita.
2. Se $z=x+iy$ con $x,y\in \mathbb{R}$ allora $$
e^{z}=e^{x}e^{iy}=e^{x}(\cos y+i\sin y).
$$
3. $|e^{iy}|=|\cos y+i\sin y|=1$, in particolare $$
|e^{x+iy}|=|e^{x}|=e^{\mathfrak{Re}(z)}
$$
4. $exp:\mathbb{C}\to \mathbb{C}^{\times}$ è surgettiva.
5. Essendo analitica, $exp$ è olomorfa.
6. $e^{z}=e^{w}$ se e solo se $z-w=2k\pi i$

---
## Logaritmo complesso
Sappiamo che $exp$ è surgettiva, però non è iniettiva, dunque non ha senso cercare un inversa globale, possiamo provare perlomeno a cercare $L:\mathbb{C}^{\times}\to \mathbb{C}$ tale che $\exp L=id_{\mathbb{C}^{\times}}$. Insiemisticamente (per *Scelta*) questa mappa esiste, ma vorremmo cercarla continua. Purtroppo dimostreremo che non esite.

*Definizione*(Rivestimento):
Una funzione continua $p:E\to X$ è un rivestimento se
1. $X$ è connesso,
2. per ogni $x \in X$ esiste un intorno $U$ di $x$ aperto detto intorno *ben rivestito*, tale che $$
p^{-1}(U)= \bigsqcup_{i \in I}W_{i},
$$
dove per ogni $i \in I$ abbiamo che $W_{i}$ è aperto in $E$ e che $p_{|_{W_{i}}}:W_{i}\to U$ è un omeomorfismo.

*Proposizione*(L'esponenziale complesso è un rivestimento):
La mappa $\exp:\mathbb{C}\to \mathbb{C}^{\times}$ è un rivestimento.

[[Gruppo fondamentale]]
#complex 