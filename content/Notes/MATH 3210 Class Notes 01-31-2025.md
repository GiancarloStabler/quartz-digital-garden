#note #abstract-algebra/vector-spaces 

#### Continuing with Direct Sums

##### Examples
2) If $V_{k}= \{  (0,\ldots,0,x_{k}, 0,\ldots,0) \in \mathbb{F}^n \}$, then $\mathbb{F}^n= V_{1} \oplus \cdots \oplus V_{n}.$
3) *Nonexample:* Let $V_{1}= \{  (X,y,0) \in \mathbb{F}^3 \}, V_{2}=\{  (0,0,z) \in \mathbb{F}^3 \}, V_{3}= \{  (0,y,y)\in \mathbb{F}^3 \}$.
	Question: $\mathbb{F}^3=V_{1}\oplus V_{2}\oplus V_{3}$?
		It is clear that $\mathbb{F}^3=V_{1}+V_{2}+V_{3}$: $(a,b,c)=(a,b,0)+(0,0,c)+(0,0,0)$. However, $(0,0,0)=(0,0,0)+(0,0,0)+(0,0,0)=(0,1,0)+(0,0,1)+(0,-1,-1).$
		Thus, $\mathbb{F}^3$ is not a direct sum of $V_{1} \oplus V_{2}, \oplus V_{3}.$

#### Proposition
Suppose $V_{1},\ldots, V_{m}$ are subspaces of $V$. Then, $V_{1}+\cdots + V_{m} = V_{1} \oplus \cdots V_{m}$ if and only if the only way to write $0$ as a sum of $v_{1}+\cdots + v_{m}$ is if all the $v_{k}$'s are $0$.

##### Proof
Homework!

#### Proposition
Suppose $U$ and $W$ are subspace of $V$, then $U+W= U \oplus W$ if and only if $U \cap W = \{  0 \}$.

##### Proof
"$\implies$"
Assume $U + W$ is a direct sum. Let $v\in U \cap W$, then $0=v+(-v)$. Since $U,W$ are vector spaces, $-v \in U \cap W$ as well. By the previous proposition, $0$ has a unique representation as a sum of elements of $U$ and $W$: $0=0+0$. Thus, $v=0$, so $U \cap W = \{ 0 \}$.

"$\impliedby$"
Assume $U \cap W = \{ 0 \}$. Suppose $u\in U$ and $w \in W$, and $u+w=0$. By previous proposition, $U+W=U \oplus W$ iff $u=w=0$.


### Finite Dimensional Vector Spaces

$V$ is a vector space over $\mathbb{F}$.

Defined [[Linear Combination]], [[Span]], [[Finite-Dimensional|Finite-Dimensionality]]

Discussed polynomial space as an example of a vector space.

