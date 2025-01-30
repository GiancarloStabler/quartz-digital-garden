#note #logic

#### Terminology About Trees
A *tree* is a partially ordered structure with a unique least element (called the root) such that for every node $x$ in the tree, the set of elements $\{ y \mid y \leq x\}$ is finite and linearly ordered.

**Root**: the node at the top of the tree (in picture).
**Predecessors**: nodes above something (in picture).
**Successors**: nodes below something (in picture).
**Leaves**: nodes with no successors.
**Branch**: a maximal linearly ordered subset.

Trees needn't be finite. This will particularly arise once we begin to work with modal logic.

In a finite tree, every branch is uniquely determined by a leaf.

#### Example: Recursive Definition

Give a recursive definition for $V(\alpha)=\#$ variables occurring in $\alpha$. 
(Count *all* occurrences ... $V(((p \implies \neg p) \vee q))=3$).

*Base:* $V( v_{i}) = 1$.

*Inductive:* $V(\neg \varphi)=V(\varphi)$, $V(\varphi * \psi)=V(\varphi)+ V(\psi)$.

Thus the final definition is,
$$
V(\alpha) = \begin{cases}
1 & \text{ if } \alpha \text{ is } v_{i}, \\
V(\varphi) & \text{ if } \alpha \text{ is } \neg \varphi,  \\
V(\varphi) + V( \psi) & \text{ if } \alpha \text{ is } (\varphi * \psi).
\end{cases}
$$

#### Unique Readability of Formulas

For each formula $\alpha$, exactly one of the following holds:
1) $\alpha$ is a proposition variable, which is uniquely determined.
2) $\alpha$ has form $\neg \varphi$ for a unique formula $\varphi$. 
3) $\alpha$ has form $( \varphi *\psi)$ where $\varphi$, $\psi$, and $*$ are uniquely determined.