#definition #logic/propositional-logic

#### Definition
We recursively define the set of finite tableau from $\Gamma$.
1) A finite signed formula tree consisting of just a labeled root node is a finite tableau from $\Gamma$.
2) If $P$ is a finite tableau from $\Gamma$ and $\sigma$ is a labeled node on $P$, then the decomposition of $\sigma$ on $P$ generates a finite tableau from $\Gamma$ using the same [[finite tableau]] rules.
3) If $P$ isa. finite tableau from $\Gamma$ and $\gamma \in \Gamma$, then we can form a new finite tableau from $\Gamma$ by adding a new node labeled $T\gamma$ to the end of each non-contradictory branch in $P$.
4) A finite signed formula tree is a finite tableau from $\Gamma \iff$ it is formed using 1) and finitely many applications of 2) and 3).

#### Examples


