[[07_Kontextfreie_Sprachen_1.pdf]]

## Definitionen und Eigenschaften
- Kontextfreie Grammatiken sind Erweiterung der regulären Grammatiken
- Produktionen sind so aufgebaut, dass auf ==linker Seite== nur ein ==einzelnes Nonterminal== steht
- Rechte Seite kann aus beliebigen Sequenz von Terminal- und Nonterminalzeichen bestehen
Grammatik ist genau dann **kontextfrei**, wenn jede Produktion die Form $l \rightarrow r$ mit $l \in V$ und $r \in (\Sigma \cup V)^*$  besitzt.
---
### Wortproblem
- für kontextfreie Sprachen entscheidbar
- lässt sich mit dem Mittel der dynamischen Programmierung effizient lösen
> [!info] 
> Dynamische Programmierung bedeutet, ein Problem in kleinere Teile zu zerlegen. Die optimale Lösung des Gesamtproblems lässt sich aus den optimalen Lösungen der Teilprobleme berechnen.

---
## Zusammenhang Kontextfreie Sprache - Chomsky-Normalform
> [!note]
> Die [[Chomsky-Normalform]] ist eine spezielle Schreibweise von kontextfreien Grammatiken.

---
## Übung
![[Schrittweise Erzeugung der Chomsky-Normalform]]