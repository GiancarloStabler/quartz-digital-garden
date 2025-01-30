#note #abstract-algebra/vector-spaces 

#### Proposition
A subset $U$ of $V$ is a [[subspace]] of $V$ if and only if $U$ satisfies:
1) $0\in U$
2) $u,w \in U$ implies $u+w \in U$.
3) $a\in \mathbb{F}$, $u\in U$ implies $au \in U$.

##### Proof
"$\implies$"
Assume $U$ subspace of $V$.  Then $U$ is a [[vector space]] with $0\in U$. Therefore, $U$ trivially satisfies conditions 1), 2), and 3).

"$\impliedby$" 
Assume $U \subseteq V$ satisfies conditions 1), 2), and 3). Clearly, $0\in U$ (by assumption), and addition and scalar multiplication are well-defined on $U$. If $u\in U$, then, by 3), $(-1) u = -u \in U$. So $U$ contains all additive inverses. Since $U \subseteq V$, any $u\in U$ is also in $V$. So the vector space properties (associativity, distributivity, commutativity, and existence of an identity) are trivially held for any elements in $U$ since they are held for those elements in the vector space $V$.


#### Example
1) For which $b\in \mathbb{F}$ is $U = \{  (x_{1},x_{2},x_{3})\in \mathbb{F}^3 \mid x_{1}=5x_{3}+b\}$ a subspace of $\mathbb{F}^3$?
	Since $0 \in U$, we must have $0=5(0)+ b$ so $b = 0$.
2) The set of differentiable real-valued functions on $\mathbb{R}$ is a subspace of $\mathbb{R}^{\mathbb{R}}$:
	1) $0\in \mathbb{R}^{\mathbb{R}}$ and $0$ is differentiable.
	2) If $f,g$ are differentiable, so is $f+g$.
	3) If $f$ is differentiable and $\lambda\in \mathbb{R}$, then $\lambda f$ is differentiable.
	$\implies$ differentiable subspace of $\mathbb{R}^{\mathbb{R}}$.
	Similarly, continuous functions are a subspace of $\mathbb{R}^{[0,1]}$.
3) The set of complex sequences with $\lim_{ k \to \infty }x_{k}=0$ is a subspace of $\mathbb{C}^{\infty}$.


#### Sums of Subspaces

##### Definition
Suppose $V_{1},V_{2},\ldots, V_{m}$ are subspaces of $V$. The sum of $V_{1},\ldots, V_{m}$ is
$$
V_{1}+ \ldots + V_{m} = \{  v_{1}+\ldots + v_{m} \mid v_{k} \in V_{k}\quad \forall k=1,\ldots,m \}.
$$
##### Example
1) Let $U = \{ (x,0,0) \in \mathbb{F}^{3} \mid x\in \mathbb{F} \}$ and $W = \{  (0,y,0) \in \mathbb{F}^3 \mid y\in \mathbb{F}\}$, then $U+W = \{ (x,y,0) \in \mathbb{F}^3 \mid x,y \in \mathbb{F} \}$.
2) Let $U = \{ (x,x,y,y) \in \mathbb{F}^4  \mid x,y \in \mathbb{F}\}$ and let $W =\{  (x,x,x,y) \in \mathbb{F}^4 \mid x,y \in \mathbb{F}\}$. Then we claim $U+W = \{  (x,x,y,z) \in \mathbb{F}^4 \mid x,y,z \in \mathbb{F} \}$.

##### Proposition
$V_{1}+\cdots+V_{m}$ is the *smallest* subspace of $V$ containing $V_{1},V_{2},\ldots, V_{m}$.


### Defined [[Direct Sum|Direct Sums]]

We know $w\in V_{1} + \cdots + V_{m}$ can be expressed as $w=v_{1}+\cdots +v_{m}$. 