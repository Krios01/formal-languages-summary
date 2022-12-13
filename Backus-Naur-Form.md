Bei der Backus-Naur-Form handelt es sich um eine ==alternative Beschreibungsform== für kontextfreie Grammatiken.
Sie ist der De-facto-Standard für die Beschreibung von Programmiersprachen.
> [!note]
> Als Ableitungssymbol wird ::= anstelle von -> verwendet.

Es gibt Spezialkonstrukte, wie z.B. die Strichnotation, um Produktionen mit gleicher linker Seite zu einer einzigen Regel zusammenzufassen.
## Optionales Einfügen
$$A ::= r_1\ [r_2]\ r_3$$
Das Wort in den eckigen Klammern kann optional einmal eingefügt werden.
## Wiederholtes Einfügen
$$A ::= r_1\ \{r_2\}\ r_3$$
Das Wort in den geschweiften Klammern kann beliebig oft wiederholt werden.
## Reduktion der Backus-Naur-Form auf normale Produktionen
### Auswahl
$$
\begin{aligned}
	A &::= r1\ |\ ...\ |\ r_n \\
	A &\rightarrow r1 \\
	A &\rightarrow\ ... \\
	A &\rightarrow r_n \\
\end{aligned}
$$
### Optionales Einfügen
$$
\begin{aligned}
	A &::= r_1\ [r_2]\ r_3 \\
	A &\rightarrow r_1\ r_3 \\
	A &\rightarrow r_1\ r_2\ r_3 \\
\end{aligned}
$$
### Wiederholtes Einfügen
$$
\begin{aligned}
	A ::= r_1\ \{r_2\}\ r_3 \\
	A \rightarrow r_1\ B\ r_3 \\
	B \rightarrow B\ r_2\ |\ \epsilon 
\end{aligned}
$$

