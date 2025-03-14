#theorem #abstract-algebra/ring-theory/polynomials 

#### Intuition
The division algorithm for [[Polynomial|polynomials]] has analogues in other [[Ring|rings]].

#### Formal Statement
Suppose $p,s \in P(\mathbb{F})$ with $s \neq 0$, then $\exists ! q,r \in P(\mathbb{F})$ such that,
$$
p = sq + r \text{ and } \deg r < \deg s.
$$

#### Proof
Assume $\deg p = n + \deg s = m$. If $n < m$, then $p = s \cdot 0 + p$ works. Assume $n \geq m$. Then the list,
$$
1,z,\ldots, z^{m-1}, s, sz, \ldots, sz^{n-m}
$$
is [[linear independence|linearly independent]] in $P_{n}(\mathbb{F})$ and has length $n+1 = \dim P_{n}(\mathbb{F})$. Thus the list is a basis. Since $p \in P_{n}(\mathbb{F})$, $\exists ! a_{0},\ldots, a_{m-1},b_{0},\ldots, b_{n-m}$ such that $p = a_{0} + a_{1}z+\cdots + a_{m-1}z^{m-1}+ b_{0}s+b_{1}sz+ \cdots +b_{n-m}sz^{n-m}$. Therefore,
$$
p=(a_{0}+\cdots+ a_{m-1}z^{m-1})+ s(b_{0}+ \cdots + b_{n-m}z^{n-m}). \qquad \qquad \square
$$

#### Corollaries