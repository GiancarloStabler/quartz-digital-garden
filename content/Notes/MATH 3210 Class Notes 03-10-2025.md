#note #abstract-algebra/vector-spaces 

### Eigenvectors and Values
#### Recall
For $\lambda \in \mathbb{F}$, an eigenvalue of $T \in \mathscr{L}(V)$, $v \neq 0$ an eigenvector associated to $\lambda \implies Tv = \lambda v$ if and only if $T - \lambda I$ is not injective, surjective, or invertible.

#### Theorem 1
Eigenvectors corresponding to distinct eigenvalues are linearly independent.

##### Proof
Suppose the above is not true for the sake of contradiction. Then there exists some smallest $m \in \mathbb{Z}_{\geq 0}$ such that the list of eigenvectors $v_{1},\ldots,v_{m}$ corresponding to distinct eigenvalues $\lambda_{1},\ldots,\lambda_{n}$ is linearly dependent. Note that $m \geq 2$ since eigenvectors are non-zero. Thus, $\exists a_{i}\in \mathbb{F}$ (none zero) such that 
$$
\begin{align*}
a_{1}v_{1} + \cdots + a_{m}v_{m} &= 0, \\
(T-\lambda_{m}I)(a_{1}v_{1}+ \cdots + a_{m}v_{m}) &= (T-\lambda_{m}I)0, \\
a_{1}(T-\lambda_{1}I)v_{1} + \cdots + a_{m}(T-\lambda_{m}I)v_{m} &= 0, \\
a_{1}(\lambda_{1}-\lambda_{m})v_{1}+ \cdots + a_{m}(\lambda_{m} - \lambda_{m})v_{m} &= 0, \\
a_{1} (\lambda_{1}-\lambda_{m}) v_{1} + \cdots + a_{m-1}(\lambda_{m-1}-\lambda_{m})v_{m-1} &= 0.
\end{align*} 
$$
Thus, we have found a smallest linearly independent list, a contradiction to the minimality of $m$. $\qquad \qquad \square$

##### Corollary
If $V$ is finite-dimensional, then any operator on $V$ has at most $\dim V$ distinct eigenvalues.


#### Operators
Operators are interesting because we can raise them to powers. If $T \in \mathscr{L}(V)$, then $TT$ makes sense, and is also an operator on $V$.
##### Notation: Suppose $T \in \mathscr{L}(V)$, and $m \in \mathbb{Z}_{\geq 0}$,then,
- $T^m = \underset{m \text{ times}}{T \cdots T}$ .
- $T^0 = I$.
- If $T$ is invertible, then $T^{-m} = (T^{-1})^m$.
##### Properties:
- $T^mT^n = T^{m+n}$.
- $(T^m)^n = T^{mn}$

If $T \in \mathscr{L}(V)$ and $p \in P(\mathbb{F})$ given by $p(z) = a_{0} + a_{1} z + a_{2}z^2 + \cdots + a_{m}z^m$, then $p(T) = a_{0}I + a_{1}T + a_{2}T^2 + \cdots + a_{m}T^m \in \mathscr{L}(V)$.

##### Example 1
Let $D \in \mathscr{L}(P(\mathbb{R}))$ be the differentiation operator $p(x) = 7 -3x+5x^2$. Then $P(D) = 7I -3D + 5D^2$. If $q\in P(\mathbb{R})$, then $(p(D))(q) = 7q -3q' -5q''$.

#### Definition 1
If $p,q \in P(\mathbb{F})$, then $pq \in P(\mathbb{F})$ and is defined by $(pq)(z) = p(z)q(z)$.

##### Proposition 1
$(pq)(T) = p(T)q(T) = q(T) p(T) = (qp)(T)$, so this is commutative.

We saw earlier, $\operatorname{null}(T)$, $\operatorname{range}(T)$ are invariant subspaces under $T \in \mathscr{L}(V)$.

##### Proposition 2
If $T \in \mathscr{L}(V)$ and $p \in P(\mathbb{F})$, then $\operatorname{null}(T)$ and $\operatorname{range}(T)$ are invariant under $T$.

##### Example 2
Let $T \in \mathscr{L}(\mathbb{F}^{\infty})$ be the backshift operator. What are the eigenvectors of $T$? $(a_{1},a_{2},\ldots)$ an eigenvector if $(a_{1},a_{2},\ldots) \neq (0,0,\ldots)$ and $T(a_{1},a_{2},a_{3},\ldots) = \lambda(a_{2},a_{3},\ldots)$.

###### Note
$T(c,c,\ldots) = 1 \cdot (c,c,\ldots)$. So anything of the form $(c,c,\ldots)$ is an eigenvector associated to $1 = \lambda$. Also, $\lambda=0$ is an eigenvalue for everything else.

##### Example 3
Let $D \in \mathscr{L}(P(\mathbb{R}))$ be the differentiation operator. What are the eigenvalues? If $\lambda$ is an eigenvalue, then, 
$$
Dp = \lambda p \text{ for some } p \neq 0.
$$
Thus, $p' = \lambda p$ for some $p \neq 0$. No nonzero $p$ satisfies this, so $\lambda = 0$ is the only eigenvalue.

##### Example 4
Let $T \in \mathscr{L}(P(\mathbb{R}))$ be $(Tp)(x)=xp'(x)$. What are the eigenvalues and vectors?
$$
xp'(x) = \lambda p(x)?
$$
$x^{\lambda}$ (vectors) works for $\lambda = 1,2,3,\ldots$ (values).

