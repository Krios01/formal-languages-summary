## Übung
### Gegeben:
$$
\begin{align}
	G &:= (\{S,A,B\},\{a,b\},P,S) \\
	S &\rightarrow AB\ |\ ABA \\
	A &\rightarrow aA\ |\ a \\
	B &\rightarrow Bb\ |\ \epsilon
\end{align}
$$
### Vorgehen:
Ausgangslage:
$$
\begin{align}
	S & \rightarrow AB \\
	S & \rightarrow ABA \\
	A & \rightarrow aA \\
	A & \rightarrow a \\
	B & \rightarrow Bb \\
	B & \rightarrow \epsilon \\
\end{align}
$$
**1. Schritt: Basis-Normalisierung:** 
- Epsilon entfernen
- b hinzufügen, da man Terminal b braucht
$$
\begin{align}
	S & \rightarrow AB \\
	S & \rightarrow ABA \\
	S & \rightarrow A \\
	A & \rightarrow aA \\
	A & \rightarrow a \\
	B & \rightarrow Bb \\
	B & \rightarrow b \\
\end{align}
$$
**Zwischenschritt:**
- Zusammenfassung aller Ableitungen der Variablen
$$
\begin{align}
	S & \rightarrow AB, aA, a, ABA, AA \\
	A & \rightarrow aA,a \\
	B & \rightarrow Bb,b \\
\end{align}
$$
**2. Schritt:** 
- Terminalzeichen überbrücken 
- Anforderung: rechts nur Nonterminale oder ein Terminal
$$
\begin{align}
	S & \rightarrow AB \\
	S & \rightarrow XA \\
	S & \rightarrow a \\
	S & \rightarrow ABA \\
	S & \rightarrow AA \\
	\\
	A & \rightarrow XA \\
	A & \rightarrow a \\
	\\
	B & \rightarrow BY \\
	B & \rightarrow b 
\end{align}
$$
**3. Schritt:** 
- Finale Form 
- rechts zwei Nonterminale oder ein Terminal
$$
\begin{align}
	S & \rightarrow AB \\
	S & \rightarrow XA \\
	S & \rightarrow a \\
	S & \rightarrow ZA \\
	\\
	Z & \rightarrow AB \\
	\\
	A & \rightarrow XA \\
	A & \rightarrow a \\
	\\
	B & \rightarrow BY \\
	B & \rightarrow b \\
	\\
	X & \rightarrow a \\
	Y & \rightarrow b
\end{align}
$$
