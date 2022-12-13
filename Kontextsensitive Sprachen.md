- Auf der linken Seiten einer Produktion kann eine beliebige Kombination aus Termianl- und Nonterminalzeichen stehen
### Einschränkung
- Anwendung einer Produktion darf nicht zu einer Verkürzung der Zeichenkette führen
- Ausnahme: das leere Wort $\epsilon$ wird direkt aus dem Startsymbol abgeleitet
### Konstruktion
1. Neben dem Startsymbol S werden drei Nonterminale A, B und C eingeführt
   -> stellvertretend für Terminalzeichen a, b und c
2. Durch neue Produktionen werden benötigte Anzahl A's, B's und C's erzeugt. Sidn ungeordnet und müssen in Reihenfolge gebracht werden.
   -> Um Sortierung zu gewährleisten, wird Grammatik um weitere Produktionen erweitert.
3. Zum Schluss werden Produktionen benötigt, die aus den Nonterminalen A, B und C die Terminalzeichen a, b und c erzeugen. Ersetzung darf nur dann erfolgen, wenn Nonterminale in der richtigen Reihenfolge angeordnet sind.
   -> Um das zu Erreichen, werden Eigenschaften der kontextsensitiven Grammatiken verwendet, dass Terminalzeichen auch auf der linken Seite einer Produktion stehen dürfen.

## Übung: Ableitung des Worts $aaabbbccc$ 
![[Pasted image 20221212171608.png]]
$$
\begin{aligned}
	S &\rightarrow SABC \\
	SABC &\rightarrow SABCABC \\
	SABCABC &\rightarrow abcABCABC \\
	abcABCABC &\rightarrow abAcBCABC \\
	abABcCABC &\rightarrow abABcACBC \\
	abABcACBC &\rightarrow abABcABCC \\
	abABcABCC &\rightarrow abABAcBCC \\
	abABAcBCC &\rightarrow abABABcCC \\
	abABABcCC &\rightarrow abAABBcCC \\
	abAABBcCC &\rightarrow aAbABBcCC \\
	aAbABBcCC &\rightarrow aAAbBBcCC \\
	aAAbBBcCC &\rightarrow aaAbBBcCC \\
	aaAbBBcCC &\rightarrow aaabBBcCC \\
	aaabBBcCC &\rightarrow aaabbBcCC \\
	aaabbBcCC &\rightarrow aaabbbcCC \\
	aaabbbcCC &\rightarrow aaabbbccC \\
	aaabbbccC &\rightarrow aaabbbccc 
\end{aligned}
$$
