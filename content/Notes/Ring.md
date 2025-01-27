#definition #abstract-algebra/ring-theory 

Rings generalize [[Field|fields]].
#### Definition
We define $(R, +, \cdot)$ as a ring if $R$ is a set and,
1) $(R, +)$ is a commutative group (identity element $0=0_{R}$).
2) $\cdot$ is an operation on $R$:
	- $\cdot$ is associative.
	- Distributivity holds
		- $a \cdot (b + c) = a \cdot b + a \cdot c$.
		- $(a+b) \cdot c = a \cdot c + b \cdot c$.

Furthermore, if,
- $\cdot$ is commutative, we say $R$ is a *commutative* ring.
- $\cdot$ has identity element $1_{R} = 1$, say $R$ is a *unital* ring.
- $R$ is unital and $\forall x \neq 0,\ \exists x ^{-1} \in R$, $x \cdot x ^{-1} = x ^{-1} \cdot x = 1_{R}$, say $R$ is a *division* ring.
- $R$ is a commutative division ring, say $R$ is a [[field]].

#### Examples
1) $Q = \{ a + bi + cj + dk \mid a,b,c,d \in \mathbb{R} \}$ is the quaternion division ring.

