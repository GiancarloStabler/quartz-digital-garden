#definition #abstract-algebra/vector-spaces 

#### Definition
A vector space (over a field $\mathbb{F}$) is a set $V$ along with an addition and scalar multiplication satisfying the following:
1) **Commutativity**. $u+v = v+u$ for all $u,v \in V$.
2) **Associativity**. $u+(v+w)= (u+v)+w$, and $a(bv)=(ab)v$ for all $u,v,w \in V$ and all $a,b \in \mathbb{F}$.
3) **Additive Identity**. $\exists 0 \in V$ such that $0+v = v$ for all $v\in V$.
4) **Additive Inverse**. $\forall v\in V$, $\exists w \in V$ such that $v+w = 0$. 
5) **Multiplicative Identity**. $1_{\mathbb{F}}v=1v=v$ for all $v\in V$.
6) **Distributivity**. $a(u+v) = au + av$ and $(a+b)v = av+bv$ for all $a,b \in \mathbb{F}$ and $u,v \in V$.

#### Addition
An addition on a set $V$ is a function ($+$) that assigns an element $u+ v \in V$ to each pair of elements $u,v \in V.$

#### Scalar Multiplication
A scalar multiplication on $V$ is a function that assigns an element $\lambda v \in V$ to each $\lambda \in \mathbb{F}$, and $v\in V$.

#### Properties
- A vector space has a unique additive identity. ([[MATH 3210 Class Notes 01-24-2025#Proof 1|Proof]])
- Every element of $V$ has a unique additive inverse. ([[MATH 3210 Class Notes 01-24-2025#Proof 2|Proof]])

#### Examples
1) Let $\mathbb{F}^{\infty} = \{ (x_{1},x_{2},\ldots) \mid x_{k} \in \mathbb{F} \}$ where vector addition and scalar multiplication are defined coordinate-wise is a vector space (over $\mathbb{F}$).
2) Let $S$ be any set. Define $\mathbb{F}^S = \{ f \mid f:S \to \mathbb{F} \}$. For $\lambda \in \mathbb{F}$, $f,g\in \mathbb{F}^S$, define
	- $(f+g)(x)= f(x)=g(x)$.
	- $(\lambda f)(x) = \lambda f(x)$.


#### Related
- [[Subspace]]