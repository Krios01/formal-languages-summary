[[07_Kontextfreie_Sprachen_1.pdf#page=32]]

Zu jeder kontextfreien Grammatik gibt es eine äquivalente kontextfreie Grammatik in Chomsky-Normalfom.

Wann liegt eine Grammatik in der Chomsky-Normalform vor?
	Wenn alle Produktionen die Form$$
	\begin{aligned}
	S &\rightarrow \epsilon, \\
	A &\rightarrow \sigma, \\
	A &\rightarrow BC
	\end{aligned}$$besitzen mit $$
	\begin{aligned}
	A &\in V, \\ 
	B, C &\in V\backslash\{S\}, \\ 
	\sigma &\in \Sigma
	\end{aligned} 
	$$
### Sonderform der Produktionen
> [!info]
> Die Produktion $S \rightarrow \epsilon$ ist erlaubt, wobei dann das Startsymbol S nicht rekursiv sein darf.
### Aufbau der Produktionen
Auf der rechten Seite stehen:
- genau zwei Variablen oder 
- genau ein Terminalzeichen

### Anwendungsfall der Chomky-Normalform:
- Beweisführung CYK-Algorithmus
- Beweisführung Pumping Lemma

Zu beachten:
- Obwohl die Gleichungen verändert werden, muss trotzdem garantiert werden, dass die gegebenen Wörter mit den neuen Gleichungen gebildet werden können

Welche Schritte sind notwendig, um eine kontextfreie Grammatik G mit $\epsilon \notin L (G)$ in Chomsky-Normalform zu überführen?
	Basis-Normalisierung
	Terminalzeichen überbrücken
	Produktionen aufspalten

### Äquivalenz von Grammatiken
> [!important]
> Zwei Grammatiken $G$ und $G'$ werden als äquivalent bezeichnet, wenn sie dieselbe Sprache erzeugen, d.h. wenn gilt $L(G) = L(G')$

**Beispiel:** 
Grammatik $G_0$ mit den Produktionen 
$$S \rightarrow aSb\ |\ \epsilon$$
und die Grammatik G1 mit den Produktionen 
$$ \begin{aligned}
S &\rightarrow C \\
C &\rightarrow D \\
E &\rightarrow ab \\
D &\rightarrow S\ |\ aSb\ |\ aF\ |\ \epsilon  
\end{aligned}$$
sind äquivalent, denn beide erzeugen die Sprache $\{ a^nb^n | n \in \mathbb{N} \}$. 
## 1. Basis-Normalisierung
> [!important]
> Sei $G = (V, T, P, S)$ eine kontextfreie Grammatik. Man bezeichnet die Grammatik als basisnormalisiert, wenn sie keine nutzlosen Variablen, kein rekursives Startsymbol, keine Epsilon-Produktionen außer $S \rightarrow \epsilon$ und keine Kettenproduktionen enthält.
### Nutzlose Variablen
Sei $G = (V, T, P, S)$ eine kontextfreie Grammatik und sei $A = V \cup T$. Eine Variable $X \in V$ heißt 
- erreichbar, wenn $S \rightarrow uXv$ mit $u, v \in A^*$ gilt, 
- produktiv, wenn $X \rightarrow w$ mit $w \in T^*$ gilt, 
- nutzlos, wenn $X$ nicht erreichbar oder nicht produktiv ist.
### Rekursives Startsymbol


![[Schrittweise Erzeugung der Chomsky-Normalform]]