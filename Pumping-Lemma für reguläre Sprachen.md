[[05_Regulaere_Sprachen.pdf#page=32]]

- Abgesehen von der letzten Regelanwendung, wird in jedem Ableitungsschritt ein Terminalzeichen und ein neues Nonterminal erzeugt.
- Nonterminal steht immer an letzter Stelle. Begrenzt die Auswahl der im nächsten Schritt anwendbaren Regeln.
- Wirkt wie ein Zustandsspeicher, der einen Rückschluss auf die bisher erzeugten Zeichen erlaubt.
- Da die Menge der Nonterminale endlich ist, lassen sich während der Erzeugung eines Wortes nur endlich viele Zustände unterscheiden.
- Das ist einer der grundlegenden Limitierungen von regulären Sprachen.

- Pumping Lemma kann zeigen, dass **Sprache nicht regulär ist**
- Kann aber nicht zeigen, dass Sprache regulär ist.

### Formale Definition:
Sei L eine von einem endlichen Automaten erkannte Sprache. 
Dann existiert eine natürliche Zahl $n \in \mathbb{N}$, dass jedes Wort $w \in L$ mit $|w| \ge n$ zerlegt werden kann in drei Teilwörter $w = xyz$.
1. $|xy| \le n$
2. $y \ne$ leeres Wort
3. $xy^{i} \in L$ für alle $i \ge 0$
### Beispiel:
Beweise, dass die Sprache nicht regulär ist.
**Gegeben:** $a^{n}b^{n}$ mit $n \in \mathbb{N}$
**Gesucht:** Wort in der Sprache $a^{n}b^{n}$, dass das Pumping Lemma verletzt.

**Allgemeiner Lösungsweg:** 
w $\in$ Sprache L
Wort w = $a^{m}b^{m}$, w $\in$ L, $|w| \ge m$ 
w = xyz, y $\ne$ leeres Wort, $|xy| \le m$ 

Zerlegung:
x = $a^{i}$ 
y = $a^{j}$
z = $a^{m-i-j}b^{m}$

y -> y²: $a^{j}a^{j} = a^{2j}$ 
w = xyyz
$w = a^{i}a^{j}a^{j}a^{m-i-j}b^{m} = a^{i+j+j+m-i-j}b^{m} = a^{j+m}b^{m}$  
Da |a| > |b|, liegt das Wort nicht in der Sprache.

**Lösungsweg mit Beispiel:**
y = y² 
1. Fall:
	y = aabb -> y² = aabbaabb
	x = leeres Wort oder a, aa, aaa, ...
	z = leeres Wort oder b, bb, bbb, ...
	aabbaabb liegt nicht in der Sprache!

2. Fall:
	y = a, aa, aaa, ... -> y = aa
	x = a
	z = bbb
	y -> y²: y² = aaaa
	$\omega$ = a aaaa bbb -> liegt nicht in der Sprache!

3. Fall:
	y = b, bb, bbb, ... -> y = bb
	x = aaa
	z = b
	y -> y²: y² = bbbb
	$\omega$ = aaa bbbb b -> liegt nicht in der Sprache!

Es ist nicht möglich y aufzupumpen. Die Sprache ist nicht regulär.