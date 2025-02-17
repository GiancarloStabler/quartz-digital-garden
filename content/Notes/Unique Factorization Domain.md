#definition #abstract-algebra/ring-theory 

#### Definition
We call $R$ a unique factorization domain if,
1) $\forall r\in R$, $r\neq 0$, unit factors as $r=x_{1}\cdots x_{n}$ for some $n \geq 1$.
2) $(*)$ is unique up to commuting $x_{i}$ or multiplying them by units.

#### Examples
- $\mathbb{Z}$, fields $F$, Euclidean domains, principal ideal domains (eg. $F[x]$) are all unique factorization domains.
- $\mathbb{Z}[i\sqrt{ 3 }]$ is not a unique factorization domain.
	- Claim: $2 \cdot 2 = 4 = (1 + i \sqrt{ 3 })(1-i \sqrt{ 3 })$ is a non-unique factorization of $4 = 4 + 0i\sqrt{ 3 }$.

#### Related
- [[Irreducible]]