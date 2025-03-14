#note #abstract-algebra/vector-spaces 

### Refresher on [[Polynomial|Polynomials]]

#### Definition 1
Suppose $z=a+bi \in \mathbb{C}$. Then,
$$
a = \mathrm{Re}z = \text{ real part of } z
$$
$$
b = \mathrm{Im} z = \text{ imaginary part of } z
$$

So $z = (\mathrm{Re} z) + (\mathrm{Im}z)i$.

#### Defined [[Complex Conjugate]]
#### Defined [[Modulus (Absolute Value)]]

#### Theorem 1
Let $w,z \in \mathbb{C}$. Then,
- $z + \bar{z} = 2(\mathrm{Re} z)$.
- $z - \bar{z} = 2(\mathrm{Im}z)i$.
- $z\bar{z} = |z|^2$.
- $\overline{w+z}= \bar{w} + \bar{z}$.
- $\bar{\bar{z}}=z$.
- $|\mathrm{Re}z| \leq |Z|$ and $|\mathrm{Im}z| \leq |z|$.
- $|\bar{z}| = |z|$.
- $|wz| = |w| \cdot |z|$.
- $|w+z| \leq |w| + |z|$ (triangle inequality).

#### Defined [[Root (Zero) of a Polynomial]]

##### Theorem
Suppose $m$ is a positive integer and $p \in P(\mathbb{F})$ of degree $m$. Then $p$ has at most $m$ [[Root (Zero) of a Polynomial|zeros]] in $\mathbb{F}$.

###### Proof (Sketch)
If $\lambda \in \mathbb{F}$ is a zero, then $\exists q \in P(\mathbb{F})$ with degree $m-1$ such that $p(z) = (z- \lambda)q(z)$. Use induction on $m$. $\qquad \qquad \square$

#### [[Division Algorithm (Polynomials)]]

#### [[Fundamental Theorem of Algebra]]

#### Theorem 2
Suppose $p \in P(\mathbb{C})$ is a polynomial with real coefficients. If $\lambda \in \mathbb{C}$ is a zero of $p$, then so is $\bar{\lambda}$.

#### Theorem 3
Suppose $p \in P(\mathbb{R})$ is a non-constant polynomial. Then, $p$ has a unique factorization (up to order) of the form,
$$
p(x) = c(x-\lambda_{1}) \cdots (x-\lambda_{m})(x^2 + b_{1}x+c_{1})\cdots(x^2+b_{M}x + c_{M}),
$$
where $c,\lambda_{1},\ldots, \lambda_{m}, b_{1},\ldots, b_{M}, c_{1},\ldots, c_{M} \in \mathbb{R}$ and $b_{k}^2 < 4c_{k}$ for all $k=1,\ldots, M$.

##### Proof (Sketch)
Imagine $p \in P(\mathbb{C})$. If all the zeros are real numbers, we get our factorization and $M=0$ by the [[Fundamental Theorem of Algebra]]. If $\lambda \in \mathbb{C}$ is a zero, so is $\bar{\lambda}$ by Theorem 2. So,
$$
p(x) = (x-\lambda)(x-\bar{\lambda}) q(x) = (x^2-2(\mathrm{Re} \lambda) x + |\lambda|^2)q(x). \qquad \square
$$
