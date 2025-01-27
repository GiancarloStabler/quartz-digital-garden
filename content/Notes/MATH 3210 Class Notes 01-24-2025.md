#note #linear-algebra 

#### Defined [[Vector Space|Vector Spaces]]

#### Proposition 1
A vector space has a unique additive identity.
##### Proof 1
By the [[Vector Space#Definition|3rd axiom]] of a vector space, we know there is at least one $0\in V$. Assume for that sake of contradiction there are two zeros: $0$ and $0'$. Because $0'$ is an additive identity, $0=0+0'$, and since $0$ is an additive identity, $0=0'$. Therefore, the additive identity is unique.

#### Proposition 2
Every element of $V$ has a unique additive inverse. 
##### Proof 2
Assume $v\in V$ has 2 inverses: $w$ and $w'$.
Then $w=w+0=w + (v+w')=(w+v)+w'=0+ w' = w'$, so $w=w'$, and every element of $V$ has a unique additive inverse.

#### Notation 
Now that we know additive inverses are unique, let
- $-v$ be the additive inverse of $v$.
- $w-v=w+(-v)$.

#### Defined [[Subspace|Subspaces]]