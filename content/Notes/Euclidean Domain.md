#definition #abstract-algebra/ring-theory #abstract-algebra/field-theory

#### Definition
We say that an integral domain $R$ is a Euclidean domain if we can define a norm $N: R \to \mathbb{Z} \cup \left\{ 0 \right\}$ such that $N(0) = 0$ and for any $a,b \in R$, we have that there exist $q,r \in R$ such that,
$$
a = qb + r \text{ with } r = 0 \text{ or } N(r) < N(b).
$$
Thus we can think of a Euclidean domain as an integral domain on which we can define a division algorithm similar to that of $\mathbb{Z}$ or $\mathbb{F}[x]$.

#### Notes
- $b \mid a$ if and only if $a \in (b)$ if and only if $(a) \subseteq (b)$.
#### Examples


