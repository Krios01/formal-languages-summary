[[02_Aufgabenblatt.pdf]]
# Aufgabe 1
[[Grammatiken]]
Gegeben sei die folgende Grammatiken: 
$$
\begin{aligned}
	G &= (T,\ V,\ S,\ P) \\
	mit\ T &:= \{ a,\ b,\ c,\ d \}, \\
	V &:= \{ S,\ A,\ D,\ M \} \\
	P &:= \{ S \rightarrow AMD\ |\ M,\ A \rightarrow AA\ |\ a,\ D \rightarrow DD\ |\ d,\ M \rightarrow bMc\ |\ \epsilon \}
\end{aligned}
$$
S -> aMD -> aMd -> ad
S -> M -> bMc -> bc
S -> AMD -> AAMD -> aAMD -> aaMD -> aaD -> aad
$$
L = \{ w \in \{ a,b,c,d \}^*\ |\ (a^{x}b^{y}c^{y}d^{z}) \}
$$

# Aufgabe 2
[[Pumping-Lemma für reguläre Sprachen]]
Gegeben sei die Sprache $L = \{ w \in \{a,b\}^*\ | \text{ w enthält gleich viele a wie b}\}$
Zeigen Sie mit Hilfe des Pumping-Lemmas, dass L nicht regulär ist.

$$ 
\begin{aligned}
	w &= \{ a, b \}^{m} \\
	|w| &\ge m \\
	w = xyz,\ y &\ne \text{leeres Wort},\ |xy| \le m \\
	x &= a^{i} \\
	y &= a^{j} \\
	z &= a^{m-i-j}b^{m} \\
	y \rightarrow y^{2}: a^{j}a^{j} &= a^{2j} \\
	w &= xyyz \\
	w &= a^{i}\ a^{2j}\ a^{m-i-j}b^{m} \\
	w &= a^{j+m}\ b^{m} \\
\end{aligned}
$$
Da |a| > |b|, liegt w nicht in der Sprache L. Somit ist gezeigt, dass L nicht regulär ist. 
q.e.d.
# Aufgabe 3
[[Pumping-Lemma für reguläre Sprachen]]
$$
\begin{aligned}
	wcw^{R} &= abab\ c\ baba \\
	x &= ab \\
	y &= abc \\
	z &= baba \\
	y \rightarrow y²: y² &= abcabc \\
	x y² z &= aba\ abcabc\ baba
\end{aligned}
$$
$xy²z$ liegt nicht in der Sprache L. Somit ist gezeigt, dass L nicht regulär ist.
q.e.d.

# Aufgabe 4
Gegeben ist die Sprache
$$
L = \{ w_1w_2 \in \sum*\ |\ w_1 \in \{a,b\}^*, w_2 \in \{b,c\}^*, \#_aw_1 + \#_bw_1 = \#_bw_2 + \#_cw_2 \}
$$
für das Alphabet $\sum = \{a,b,c\}$ 
$\#_xw$ Häufigkeit des Vorkommens eines Zeichens $x \in \sum$ in einem Wort $w \in \sum*$ an
### 1. Zeigen Sie, dass L nicht regulär ist.
[[Pumping-Lemma für reguläre Sprachen]]
$$ 
\begin{aligned}
w_1 &= abab\ bcbc \\
x &= ab \\
y &= abb \\
z &= cbc \\
y \rightarrow y²: y² &= abbabb \\
w_2 &= xy²z = ab\ abbabb\ cbc \\
\#_aw_1 + \#_bw_1 &= \#_bw_2 + \#_cw_2 \\
3 + 6 &\ne 6 + 2
\end{aligned}
$$
$w_2$ liegt nicht in der Sprache L. Somit ist gezeigt, dass L nicht regulär ist.
q.e.d
### 2. Geben Sie eine Chomsky-2-Grammatik an, durch die die Sprache L erzeugt werden kann.
[[Chomsky-Hierarchie]]
$$
\begin{aligned}
	G&(T, V, S, P) \\
	T &= \{a, b, c\}\\
	V &= \{A, B, C, S\} \\
	P &= \{S \rightarrow ASB\ |\ \epsilon,\ A \rightarrow a\ |\ b,\ B \rightarrow b\ |\ c\}
\end{aligned}
$$


