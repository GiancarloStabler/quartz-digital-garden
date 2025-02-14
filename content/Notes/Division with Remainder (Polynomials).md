#theorem #abstract-algebra/ring-theory/polynomials

#### Intuition
Similarly to how we have division with remainder in other rings ($\mathbb{Z}, \mathbb{Z}[\sqrt{ 2 }]$, etc.), we have unique division in the ring of polynomials.

#### Formal Statement
For [[Ring of Polynomials|polynomials]] $P,Q \in R[x]$, $Q \neq 0$. Assume either
1) $R = F$ is a field, or
2) $Q(x)$ monic ($LT(Q)=1$),
Then there exists $D(x), r(x) \in R[x]$ such that $P(x) = D(x) \cdot Q(x) + r(x)$ and $\deg r(x) < \deg Q(x)$.

#### Corollaries
1) In $F[x]$ we have Euclid's algorithm, we have $\gcd(P(x),Q(x))$ for any $P,Q$ not both $0$, computable with Euclid's algorithm, and $\exists u,v \in F[x]$ such that $u \cdot P + v \cdot Q= \gcd(P,Q)$.
2) If $I \unlhd F[x]$, then $I = (0)$ or $I = (P(x))$, $P(x)$ is the unique smallest nonnegative degree monic element in $I$. (We say $F[x]$ is an example of a P.I.D. (principal ideal domain)).