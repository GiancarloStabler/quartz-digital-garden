---
dg-publish: true
---
#theorem #abstract-algebra/group-theory 

#### Formal Statement
For a group $G$ acting on a set $X$, with $G,X$ finite, for all $x\in X$,
$$
|\operatorname{orb}_{G}(x)| = \frac{|G|}{|\operatorname{stab}_{G}(x)|}.
$$
#### Proof
Say $G = \{ g_{1},\ldots, g_{n} \}$.

$\operatorname{orb}(x) = \{ g_{1}\bullet x, \ldots, g_{n} \bullet x \}$.
From this, we have that there are at most $|G|$ elements, but that there very well may be repetitions.

When is $g_{i}\bullet x = g_{j} \bullet x$?

Precisely when $(g_{j}^{-1}g_{i})\bullet x = x \iff g_{j}^{-1}g_{i}\in \operatorname{stab}(x) \iff g_{i} \in g_{j} \operatorname{stab}(x)$ <- left coset.
Fixing $i$, $\# \{  j : g_{j} \bullet x = g_{i} \bullet x \} = |g_{j}\operatorname{stab}(x)| = |\operatorname{stab}(x)| \implies$ on list, $g_{1}\bullet x, \ldots, g_{n} \bullet x$ ($|G|$ elements), each element repeats $|\operatorname{stab}(x)|$ times. 

$\implies |\{ g_{1}\bullet x, \ldots, g_{n}\bullet x \}|= \frac{|G|}{|\operatorname{stab}(x)|}. \qquad \square$

