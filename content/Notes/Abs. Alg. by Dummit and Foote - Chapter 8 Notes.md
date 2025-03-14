#note #abstract-algebra/ring-theory/commutative-algebra #abstract-algebra/field-theory 

## Chapter 8 - Euclidean, Principal Ideal, and Unique Factorization Domains

### Section 8.1 - Euclidean Domains

#### Definition: [[Euclidean Domain]]

#### Proposition 1
Every [[ideal]] in a Euclidean Domain is principal. In particular, for any nonzero ideal $I$, we have that $I = (d)$ for some nonzero element $d \in I$ with minimal norm.
##### Proof
Let $I$ be a nonzero ideal in a Euclidean Domain $R$. Choose nonzero $d \in I$ such that $d$ has minimal norm (which must exist by the well ordering of $\mathbb{Z}$). Clearly, $(d) \subseteq I$ since $d \in I$, so it remains to show that $I \subseteq (d)$. Take $a \in I$, then by the existence of a division algorithm in $R$, we have that for $a,d$ there exist $q,r \in R$ such that,
$$
a = qd + r \text{ with } r=0 \text{ or } N(r) < N(d).
$$
Since $a,d \in I$, we have from the closure of $I$ that $q,r \in I$. Since $d$ was chosen to be the element with minimal nonzero norm in $I$, we know that $r = 0$ (otherwise $N(r) < N(d)$ wouldn't hold), so we have that $a = qd$ an element of $(d)$, so $I \subseteq (d)$. Therefore, we have that $I = (d)$. $\qquad \square$


It is by proposition 1 that we can show that some integral domains are not Euclidean Domains by showing that they have non-principal ideals.

#### Definition: [[Greatest Common Divisor (in a Ring)]]
Just like in $\mathbb{Z}$, the idea of a Euclidean Domain allows us to construct a generalized version of greatest common divisor. 

Note that $b \mid a$ iff $a \in (b)$ iff $(a) \subseteq (b)$. This ends up giving us that the greatest common divisor (if it exists) of $a,b \in R$ generates the *unique* smallest principal ideal containing $(a)$ and $(b)$.

It is important to note that not all rings have greatest common divisors.