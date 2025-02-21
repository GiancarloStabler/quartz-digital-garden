#note #abstract-algebra/vector-spaces 

#### Question 1
A [[vector space]] is a set $V$ with addition and scalar multiplication such that,
- Addition is commutative.
- There exists an additive identity ($0$).
- There exists a unique additive identity, $-v$, for all $v \in V$.
- Both addition and scalar multiplication are associative.
- Distribution laws are respected.

#### Question 2
Show $\mathcal{P}(\mathbb{R})$ satisfies the vector space axioms above.

#### Question 3
Show $\mathcal{P}_{m}(\mathbb{R})$ is a [[subspace]], $0\in \mathcal{P}_{m}(\mathbb{R})$, and it's closed under addition and scalar multiplication.

#### Question 4
We have that $V_{1}+ V_{2}= \left\{ v_{1}+v_{2} : v_{1}\in V_{1}, v_{2}\in V_{2}\right\}$. And we define $V_{1} \oplus V_{2}$ as $V_{1}+V_{2}$ if there is a unique way to write any element of $V_{1}+V_{2}$ as $v_{1}+v_{2}$.

#### Question 5
Does $V_{1}\oplus U = V_{2}\oplus U \implies V_{1}=V_{2}$? No?

#### Question 6


#### Question 7
Show $\operatorname{span}(v_{1},\ldots,v_{n})$ satisfies the necessary subspace conditions.

#### Question 8
Let $u_{1},\ldots,u_{m}$ be a list. If the list is linearly dependent, then there exists some $k$, $1\leq k\leq m$ where $u_{k}\in \operatorname{span}(u_{1},\ldots,u_{k-1})$ and $\operatorname{span}(u_{1},\ldots,u_{m})= \operatorname{span}(u_{1},\ldots,u_{k-1},u_{k+1},\ldots u_{m})$.

#### Question 9
Find which of $(1,2,3),(7,1,4),(0,1,1),(7,6,9)$ can be written as a sum of the other vectors.

$(1,2,3)$ linearly independent
$(1,2,3),(7,1,4)$ linearly independent
$(1,2,3),(7,1,4),(0,1,1)$ seem to be linearly independent 
$(1,2,3),(7,1,4),(0,1,1),(7,6,9)$ can't be linearly independent since a space of dimension 3 can have a list of at most 3 linearly independent vectors.

Note: if you are unsure, you can put the vectors into a matrix and do gaussian elimination to see if we can get to reduced row echelon form.

#### Question 10
Extend $(1,1,0),(0,1,1)$ to a basis of $\mathbb{R}^3$.

Add to the list a set of vectors that themselves form a basis of $\mathbb{R}^3$, so the list spans $\mathbb{R}^3$:
$(1,1,0),(0,1,1),(1,0,0),(0,1,0),(0,0,1)$.

Now use the [[linear dependence lemma]] to remove vectors that are in the span of the rest of the vectors, which leaves us with $(1,1,0),(0,1,1),(1,0,0)$ in this case.

#### Question 11
As we've shown, since $\mathbb{F}^3$ can be spanned by a linearly independent set of three vectors, the dimension of $\mathbb{F}^3$ is three.

#### Question 12
A vector space $T: V\to W$ is a morphism from a vector space $V$ to a vector space $W$ that respects sums and products in $V$ in $W$ (additivity and homogeneity).

#### Question 13
Only $b=0$ works in this case because any non-zero value of $b$ causes the additivity condition to not be satisfied for $T$.

For $T(a)=2a+b$, to be a linear map, we need that $T(a_{1}+a_{2})=T(a_{1})+T(a_{2})$ or equivalently $2(a_{1}+a_{2}) + b = 2a_{1}+ b + 2a_{2}+ b = 2(a_{1}+a_{2})+2b$, which is only true if $b=0$.

#### Question 14
The nullspace for $T:V\to W$ is the subset $N \subseteq T$ such that for $n\in N$, $T(n) = 0_{W}$.

The range for $T:V\to W$ is the subset $R \subseteq W$ such that for $r\in R$, there exists $v\in V$ such that $T(v)=r$.

#### Question 15
1) Multiplication by a constant $c\in \mathbb{R}$.
2) The differentiation map.
3) The identity map.
4) 