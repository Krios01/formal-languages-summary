## Typ-0 Grammatik

## Typ-1 Grammatik
![[Kontextsensitive Sprachen]]
## Typ-2 Grammatik
![[Kontextfreie Sprachen]]
## Typ-3 Grammatik
[[05_Regulaere_Sprachen.pdf]]
- unterliegt erheblichen Einschränkungen
	- linke Seite besteht aus Nonterminalen
	- rechte Seite besteht aus dem leeren Wort $\epsilon$ oder Terminalzeichen gefolgt von einem Nonterminalzeichen

### Beispiel:
$$ 
\begin{align}
S & \rightarrow aB \\
B & \rightarrow Bc \\
C & \rightarrow \epsilon \ |\ aB
\end{align}
$$