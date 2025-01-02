---
dg-publish: true
---
#proof #abstract-algebra/group-theory/p-groups  

#### Theorem
A group $( G, \cdot )$ is a [[P-group|p-group]] if and only if $|G| = p^k$ for some $k$.

#### Proof
If $( G, \cdot )$ is a p-group, and assume $\exists g\neq p$ prime, where $g\mid n = |G|$.

Cauchy's Theorem $\implies \exists g\in G, \operatorname{ord}_{}(g)=g$ not a power of $p$ (contradiction).

Conversely, if $|G|=p^k$, $g\in G \implies \operatorname{ord}_{}(g) \mid |G| = p^k \implies$ by [[Lagrange's Theorem]] that $\operatorname{ord}_{}(g)$ is a power of $p$. Thus, $G$ is a p-group. $\qquad \square$

#### Remark
If $(G,\cdot)$ is commutative with $n=p_{1}^{\alpha_{1}}\cdot \ldots \cdot p_{r}^{\alpha_{r}}$, $p_{i}$ distinct primes, $( G, \cdot )$ admits internal direct product decomposition as product of $p_{i}$-group $G[p_{i}]\leq G$, also commutative.

#### See
- [[Proof of P-group Theorem (2)]]


