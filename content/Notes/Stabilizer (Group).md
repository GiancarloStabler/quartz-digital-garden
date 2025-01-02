---
dg-publish: true
---
#definition #abstract-algebra/group-theory 

#### Definition
For $G \circlearrowleft X$ (a [[group]] $G$ acting on a set $X$) and $x\in X$, the stabilizer of $x$ with respect to $G$ is,
$$
\operatorname{stab}_{G}(x) = \{  g\in G : g\bullet x = x \}.
$$

#### Examples
1) Say $\tau \in D_{4}$ is the reflection across the $x$-axis.
	$D_{4}$ acts on a square (where the origin is the center of the square)
	$\tau$ stabilizes $(1,0)$ and $(-1,0)$ on the $x$-axis since reflecting across the $x$-axis does not change $(1,0)$ and $(-1,0)$.
	$\tau \in \operatorname{stab}((1,0))$
	$\tau\not\in \operatorname{stab}((0,1))$

#### See
- [[Note - Orbits and Stabilizers]]

