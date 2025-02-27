#note #abstract-algebra/field-theory #abstract-algebra/vector-spaces 

### [[Field Extension]]

#### Defined [[Prime Subfield]]

#### Defined [[Morphism of Field Extensions]]

#### Defined [[Degree of Extensions]]

#### Theorem
for $K \subseteq E \subseteq F$ extensions, then
$$
[F:K] = [E:K] \cdot [F:E].
$$
##### Proof
Assume: $[E:K] = n < \infty$, and $[F:E] = m < \infty$. Assume there also exists a basis $e_{1},\ldots, e_{n}\in E$ over $K$, and $f_{1},\ldots, f_{m}$ a basis over $E$. 

*Claim:* $(e_{i}\cdot f_{j})_{\underset{1 \leq j \leq m}{1 \leq i \leq n}}$ is a basis of $F$ over $K$ (this is the product in $F$).
Span: Let $f \in F \implies \exists \varepsilon_{1}, \ldots,\varepsilon_{m} \in E, f = \varepsilon_{1}f_{1}+ \cdots + \varepsilon_{m}f_{m}$ in $F$.
For all $1 \leq j \leq m$, there exists $c_{ij} \in K$ (for $1 \leq i \leq n$) such that $\varepsilon_{j} = c_{1j}e_{1} + \cdots + c_{nj}e_{n}$ in $E$ $\implies$ $f=\sum_{ij}^{}c_{ij}\cdot(e_{ifj})$ in $F$ $\implies$ the $e_{ifj}$ span $F$ over $K$.

Linear independence: Want that if...

#### Lemma 
Take some field $K$, and polynomial $P(x) = x^n + a_{n-1}x^{n-1} + \cdots + a_{0} \in K[x]$. Assume $P(x)$ is irreducible, then,
$$
{^{\textstyle K[x]}\big/_{\textstyle (P(x))}} \text{ is a field and } \left[{^{\textstyle K[x]}\big/_{\textstyle  (P(x))}}:K\right] = n.
$$

##### Remark
If $n > 1$, $P(x) \in K[x]$ monic irreducible of degree $n$ $\implies$ $P(x)$ has no roots in $K$, but $K[x]$ is a field, $\alpha \in K[x]$ is a root of $P(x)$.