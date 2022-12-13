$L = \{a^n\ b^n\ |\ n \in N_0\}$ 
$S \rightarrow C$
$C \rightarrow aSb$
$C \rightarrow \epsilon$
### Schritt 1: Basis Normalisierung
$S' \rightarrow aSb\ |\ \epsilon\ |\ ab$   
$S \rightarrow aSb\ |\ ab$  
### Schritt 2: Terminalzeichen überbrücken
$S' \rightarrow ASB\ |\ \epsilon\ |\ AB$
$S \rightarrow ASB\ |\ AB$
$A \rightarrow a$
$B \rightarrow b$ 
### Schritt 3: Produktionen aufspalten
$S' \rightarrow AX\ |\ \epsilon\ |\ AB$
$X \rightarrow SB$
$S \rightarrow AY\ |\ AB$
$Y \rightarrow SB$  