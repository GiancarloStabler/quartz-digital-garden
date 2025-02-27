#note #abstract-algebra/vector-spaces 

#### Theorem 1
If $V_{i}$ is [[finite-dimensional]], then $V_{1} \times \cdots \times V_{n}$ is finite dimensional and,
$$
\dim(V_{1} \times \cdots \times V_{n}) = \dim V_{1} + \cdots + \dim V_{n}.
$$
#### Remark 1
There is a canonical map $\Gamma: V_{1} \times \cdots \times V_{n} \to V_{1}+ \cdots + V_{n}$, given by $\Gamma(x_{1},\ldots,x_{n}) = x_{1}+\cdots + x_{n}$.

#### Theorem 2
$V_{1} + \cdots + V_{n}$ is a [[direct sum]] if and only if $\Gamma$ is injective.

##### Example 3
Suppose $T:V\to W$ is linear. 

The graph of $T$ is the subspace of $V \times W$ given by graph of $T = \left\{ (v,Tv) : v \in V \right\}.$

### Quotient Spaces

##### Notation
Let $v\in V$ and $U \subseteq V$, then $v + U$ is the subset of $V$ defined by $v + U \left\{  v+u : u \in U \right\}.$

##### Example 1
Let $U = \left\{ (x,2x) : x \in \mathbb{R} \right\} \subseteq \mathbb{R}^2$. What is $(5,1) + U$?

$v+U$ is a translate of $U$. 

#### Defined [[Quotient Space]]

##### Proposition
Suppose $U$ is a [[subspace]] of $V$ and $v,w \in V$, then $v-w \in U \iff v + U = w +U \iff (v+U) \cap (w + U) \neq \emptyset.$

#### [[First Isomorphism Theorem of Vector Spaces]]

#### Theorem
Suppose $U$ is a subspace of $V$ such that ${^{\textstyle  V}\big/_{\textstyle U}}$ is finite-dimensional, then
$$
V \simeq U \times ({^{\textstyle V}\big/_{\textstyle U}}).
$$

### Duality

#### Dual Vector Space
For some [[vector space]] $V$ over the field $\mathbb{F}$, we have that the dual vector space $V' = \mathscr{L}(V, \mathbb{F})$.

##### Example
If $V = P(\mathbb{R})$, $\mathbb{F} = \mathbb{R}$, then $\varphi(p) = 5p''(0) \in (P(\mathbb{R}))'$.