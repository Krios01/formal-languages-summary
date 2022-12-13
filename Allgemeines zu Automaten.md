### Alphabet einer Sprache
- Programme werden in Programmiersprache geschrieben
- Menge aller Zeichen, die sie zulässt, wird als Alphabet der jeweiligen Programmiersprache bezeichnet
- Zulässige Zeichen sind z.B. <, =, +, - sowie Buchstaben und Ziffern
### Wörter einer Sprache
- Wörter werden aus dem Alphabet definiert
Unterteilen sich in:
- Schlüsselwörter (while, for, if)
- Sonderzeichen (+, -, =)
- Benutzerdefinierte Bezeichner (nahme, wohnort)
- Konstanten (123, 5.19, 'r')
## 1. Phase: Lexikalische Analyse
- Zerlegung eines Programms in seine einzelnen Wörter (sog. Tokens)
- Entfernen von white spaces
- Token gibt an, zu welcher Klasse von Wörtern das Wort gehört
- Jedem Schlüsselwort ist ein eigener Token zugeordnet
- Zuordnen von Tokens wird auch als Scannen bezeichnet
## 2. Phase: Syntaktische Analyse
- Syntaxanalyse prüft, ob Reihenfolge der einzelnen Wörter (Tokens) in zugrundeliegenden Programmiersprache erlaubt sind
- Überprüfung wird auch als Parsen und die Analyseprogramme als Parser bezeichnet