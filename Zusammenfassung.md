# Themen
[[Grammatiken]]
[[Chomsky-Hierarchie]]
[[Pumping-Lemma für reguläre Sprachen]]
[[Reguläre Ausdrücke]]
[[Kontextfreie Sprachen]]
# Einstieg 
[[01_Einstieg.pdf]]
### Formale Grammatiken: 
[[01_Einstieg.pdf#page=15]]
- Ausgehend von einem Startsymbol lassen sich Produktionsregeln aus einer Regelmenge anwenden.
- Erzeugen aus dem Startsymbol neue Zeichenfolgen (Wörter).
- Können wiederum weiter ersetzt werden.
- Vorgang der **Ableitung**
### Vokabular
[[01_Einstieg.pdf#page=15]]
- Grammatik besteht aus disjunkten Vereinigung eines Alphabets von Terminalsymbolen mit einer Menge von Nichtterminalsymbolen.
- Grammatik gibt vor, welche Symbole verwendet werden können.
- Menge der Terminalsymbole definiert, welche Zeichen nicht weiter abgeleitet werden können.
- Alle Wörter zusammengenommen sind die, von der Grammatik beschriebene, formale Sprache.
- Startsymbol muss ein Nichtterminalsymbol sein.
- Zusätzliche Nichtterminalsymbole erlauben differenziertere Regeln.
### Sprachklassen (Chomsky-Hierarchie)
[[01_Einstieg.pdf#page=16]]
- Klassifizierung von Grammatiken nach der Komplexität der Regeln. 
- Dadurch Klassifizierung der formalen Sprache selbst.
Vier Stufen der **Chomsky-Hierarchie**:
- Typ 0 - Typ 3
- Je höher der Typ, desto eingeschränkter sind dabei die Regeln.
- Wenn Sprache von Typ-n-Grammatik erzeugt wurde, ist Sprache ebenfalls vom Typ n
### Nicht deterministische / deterministische endliche Automaten
[[01_Einstieg.pdf#page=21]]
deterministische Automaten:
- Für jeden Zustand existiert genau ein Übergang für jede mögliche Eingabe
 ![[Pasted image 20221113122529.png]]
nicht-deterministische Automaten:
- Für jeden Zustand kann es keinen, einen oder mehr als einen Übergang für jede mögliche Eingabe geben.
![[Pasted image 20221113122709.png]]
# Sprachen und Grammatiken
[[03_Sprachen_Grammatiken.pdf#page=4]]
Theorie der formalen Sprachen beschäftigt sich mit der systematischen Analyse,
Klassifikation und Konstruktion von Wortmengen, die über einem endlichen
Alphabet gebildet werden. 
- Alphabet Σ ist eine endliche Menge von Symbolen. 
- Jedes Element σ ∈ Σ ist ein Zeichen des Alphabets. 
- Jedes Element ω ∈ Σ* wird als Wort über Σ bezeichnet. 
- Jede Teilmenge L ⊆ Σ* ist eine formale Sprache über Σ.

