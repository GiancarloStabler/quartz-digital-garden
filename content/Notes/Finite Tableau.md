#definition #tags 

#### Definition
A finite tableau is a finite signed formula tree built recursively as follows:
1) A signed formula tree consisting of only a root is a finite tableau.
2) Let $P$ be a finite tableau and $\sigma$ be a labelled node on $P$. The decomposition of $\sigma$ on $P$ generates a new finite tableau by extending all of the leaves on $P$ below $\sigma$ according to the label of $\sigma$ using the diagrams below.
3) A finite signed formula tree is a finite tableau if and only if it is generated from $1)$ by finitely many applications of $2)$.

#### Decomposition Diagrams
$\sigma$ is at top, and $\lambda$ is a leaf below $\sigma$ (do extension below every leaf $\lambda$ extending $\sigma$).

$$
\begin{array}{c c c c c}
T\neg \alpha & F \neg \alpha & T \alpha \vee \beta & F \alpha \vee \beta & \cdots \\

\end{array}
$$
#### Examples


