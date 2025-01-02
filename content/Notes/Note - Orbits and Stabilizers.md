---
dg-publish: true
---
#note #abstract-algebra/group-theory 

[[Orbit (Group)]]
[[Stabilizer (Group)]]

#### Remark
If $( G, \cdot ) \circlearrowleft X$, we have an equivalence relation on $X$
$x \sim x'$ if $x'= g\bullet x$ for some $g\in G$.
This is indeed an equivalence relation, and $[x]= \operatorname{orb}_{G}(x)$.

#### Corollary
If $( G, \cdot ) \circlearrowleft X$,
1) $X$ is partitioned by distinct orbits.
2) $\operatorname{orb}(y)=\operatorname{orb}(x) \iff y\in \operatorname{orb}(x)$.
3) $x\in \operatorname{orb}(x)$.
4) Either $\operatorname{orb}(y) = \operatorname{orb}(x)$ or $\operatorname{orb}(y) \cap \operatorname{orb}(x) = \emptyset$ in $X$.

#### Recall
If $G \circlearrowleft G$ by conjugation, $g\in G$, we have $|[g]| = \frac{|G|}{|C_{G}(g)|}$ (where $C_{G}(g)$ is the [[centralizer]] of $g$ in $G$).

#### Recall
$x\in C_{G}(g)$ if $gx=xg \iff xgx^{-1} = g \iff x \bullet g = g$ (specifically where $\bullet$ is the action by conjugation).


For arbitrary actions, we have "[[Stabilizer (Group)|stabilizers]]".
#### Proposition
For $G\circlearrowleft X$, and $x\in X$. The stabilizer, $\operatorname{stab}_{G}(x) \leq G$, is a subgroup.

##### Proof
$e_{g}\bullet x = x \implies e_{G} \in \operatorname{stab}_{G}(x)$
$g,g' \in \operatorname{stab}_{G}(x) \implies (gg')\bullet x = g\bullet (g' \bullet x) \implies gg' \in \operatorname{stab}_{G}(x)$

Say $g\bullet x = x \implies g^{-1} \bullet (g \bullet x) = g^{-1} \bullet x$ and $g^{-1} \bullet (g \bullet x) = (g^{-1}g)\bullet x = e_{G} \bullet x = x \implies g^{-1} \in \operatorname{stab}_{G}(x). \qquad \square$

#### Remark


