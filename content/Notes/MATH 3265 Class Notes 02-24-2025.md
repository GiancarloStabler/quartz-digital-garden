#note #logic/propositional-logic 

### [[Finite Tableau]]

#### [[Tableau Rule Agreement Lemma]]

#### Example
Show $\neg ( p \wedge q) \leftrightarrow (\neg p \vee \neg q)$.

```tikz
\usepackage{circuitikz}

\begin{document}

\begin{circuitikz}
\tikzstyle{every node}=[font=\LARGE]
\node [font=\LARGE] at (4.25,13.5) {F $\neg$(p $\wedge$ q ) $\leftrightarrow$ ($\neg$ p $\vee$ $\neg$ q)};
\node [font=\LARGE] at (0,11.25) {T $\neg$ ( p $\wedge$ q)};
\draw [short] (0.25,11.75) -- (3.5,13);
\draw [short] (4.75,13) -- (8.25,11.75);
\node [font=\LARGE] at (0,8.75) {F $\neg$ p $\vee$ $\neg$ q};
\node [font=\LARGE] at (8.25,11.25) {F $\neg$ (p $\wedge$ q)};
\node [font=\LARGE] at (8,8.75) {T $\neg$ p $\vee$ $\neg$ q};
\draw [short] (0,10.5) -- (0,9.5);
\draw [short] (8.5,10.5) -- (8.5,9.5);
\node [font=\LARGE] at (0,6) {F p $\wedge$ q};
\node [font=\LARGE] at (8.25,6.25) {T p $\wedge$ q};
\node [font=\LARGE] at (6.5,3.75) {T $\neg$ p};
\node [font=\LARGE] at (9.75,3.75) {T $\neg$ q};
\node [font=\LARGE] at (6.5,1.25) {T p};
\node [font=\LARGE] at (9.75,1.25) {T p};
\node [font=\LARGE] at (6.5,-1.25) {T q};
\node [font=\LARGE] at (9.75,-1.25) {T q};
\node [font=\LARGE] at (6.5,-3.75) {F p};
\node [font=\LARGE] at (9.75,-3.75) {F q};
\draw [short] (8.5,8) -- (8.5,7);
\draw [short] (6.75,4.5) -- (8,5.5);
\draw [short] (8.5,5.5) -- (9.75,4.5);
\draw [short] (6.5,3) -- (6.5,2);
\draw [short] (6.5,0.5) -- (6.5,-0.5);
\draw [short] (9.75,0.5) -- (9.75,-0.5);
\draw [short] (6.5,-1.75) -- (6.5,-3);
\draw [short] (9.75,-1.75) -- (9.75,-3);
\draw [short] (9.75,3.25) -- (9.75,2);
\node [font=\LARGE] at (0,3.75) {F $\neg$ p};
\node [font=\LARGE] at (0,1.25) {F $\neg$ q};
\node [font=\LARGE] at (-1.5,-1.25) {F p};
\node [font=\LARGE] at (1.25,-1.25) {F q};
\node [font=\LARGE] at (-1.5,-3.75) {T p};
\node [font=\LARGE] at (1.25,-3.75) {T p};
\node [font=\LARGE] at (1.25,-6.25) {T q};
\draw [short] (0,8) -- (0,7);
\draw [short] (0,5.5) -- (0,4.5);
\draw [short] (0,3) -- (0,2);
\draw [short] (-0.25,0.5) -- (-1.25,-0.25);
\draw [short] (0.25,0.5) -- (1,-0.25);
\draw [short] (-1.5,-2) -- (-1.5,-3);
\draw [short] (1.25,-2) -- (1.25,-3);
\draw [short] (1.25,-4.5) -- (1.25,-5.5);
\draw  (-1.5,-3.75) circle (0.75cm);
\draw  (1.25,-6.25) circle (0.75cm);
\draw  (6.5,-3.75) circle (0.75cm);
\draw  (9.75,-3.75) circle (0.75cm);
\end{circuitikz}

\end{document}
```

Since all branches are contradictory, this finite tableau is a *proof* of $\neg ( p \wedge q) \leftrightarrow (\neg p \vee \neg q)$, so this formula is provable. 


#### Where Are We Going?
- $\vdash \neg (p\wedge q) \leftrightarrow (\neg p \vee \neg q)$ means:
	- There is a proof of this formula.
	- There is a contradictory tableau with root $F \neg(p \wedge q) \leftrightarrow (\neg p \vee \neg q)$.
- $\models \neg ( p \wedge q) \leftrightarrow (\neg p \vee \neg q)$ means:
	- *Every* valuation $V$ has $V ( \neg (p \wedge q) \leftrightarrow (\neg p \vee \neg q) = 1$.
	- In the truth table, this formula has value $1$ in every row.
	- This formula is a tautology.

