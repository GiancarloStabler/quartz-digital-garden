#note #abstract-algebra/vector-spaces 

### Invertibility and Isomorphisms

#### Theorem
Suppose $V,W$ are [[finite-dimensional]] [[Vector Space|vector spaces]] and $\dim V = \dim W$. If $T: \in \mathscr{L}(V,W)$, then $T$ is [[Inverse (Linear Map)|invertible]] if and only if $T$ is injective if and only if $T$ is surjective.

##### Proof
Invertible $\implies$ injective and surjective is trivial because we have already proved an earlier theorem (invertible $\iff$ injective and surjective).

Also, ETS injective $\iff$ surjective because of the theorem.

(Injective $\implies$ Surjective)
*Recall:* [[Fundamental Theorem of Linear Maps]]

Injectivity $\implies$ $\dim \operatorname{null} (T) = 0$, so then the FTLM implies that $\dim V = 0 + \dim \operatorname{range}(T) = \dim W$ by assumption. Therefore, $\dim W = \dim \operatorname{range}(T)$, so $T$ is surjective.

(Surjective $\implies$ Injective)
FTLM gives us that $\dim V = \dim \operatorname{null}(T) = \dim \operatorname{range}(T)$, so $\dim W = \dim \operatorname{null}(T) + \dim W$, so $0 = \dim \operatorname{null}(T) \implies \operatorname{null}(T) = \left\{ 0 \right\}$, so $T$ is injective.

#### Theorem
Suppose $\dim V = \dim W < \infty$, $S \in \mathscr{L}(W,V)$, $T \in \mathscr{L}(V,W)$. Then $ST = I_{V} \iff TS = I_{W}$. 

#### Defined [[Isomorphic Vector Spaces]]

##### Theorem
Two finite dimensional vector spaces over some field $\mathbb{F}$, are isomorphic if and only if they have the same dimension.

###### Proof
("$\implies$") 
Suppose $V,W$ are isomorphic. Then there exists some map $T: V \to W$ that is an isomorphism (i.e. invertible). By the Fundamental Theorem of Linear Maps, we have $\dim V = \dim \operatorname{null}(T) + \dim \operatorname{range}(T) = 0 + \dim W$.

("$\impliedby$")
Assume $\dim V = \dim W = n$. Let $v_{1}, \ldots, v_{n}$ and $w_{1}, \ldots, w_{n}$ be bases of $V,W$, respectively. Define $T \in \mathscr{L}(V,W)$ by $T(c_{1}v_{1} + \cdots + c_{n}v_{n}) = c_{1}w_{1} + \cdots + c_{n}w_{n}$. $T$ is well-defined, since $v_{i}$'s form a basis. Also, $T$ is surjective, since every element in $W$ can be written as a linear combination of $w_{1},\ldots, w_{n}$, which corresponds to some $T(v)$ by the definition of $T$. Furthermore, $T$ is injective since the nullspace of $T$ is $\left\{ 0 \right\}$. Therefore, $T$ is invertible, so $T$ is an isomorphism.

##### Corollary
If $\dim V = n$, then $V \simeq \mathbb{F}^n$. 

##### Example
1) $P_{m}(\mathbb{R}) \simeq \mathbb{R}^{m+1}$. An example isomorphism is the one below,
$$	T(a_{0} + a_{1} z + \cdots + a_{m}z^m) = \begin{bmatrix}
a_{0} \\ a_{1} \\ \vdots \\ a_{m}
\end{bmatrix}	$$
##### Notation
$\mathbb{F}^{m,n} :=$ vector space of $m$-by-$n$ matrices with coefficients in $\mathbb{F}$.
$$
\dim \mathbb{F}^{m,n} = m \cdot n
$$

If $v_{1},\ldots, v_{n}$ is a basis of $V$ and $w_{1}, \ldots, w_{m}$ is a basis of $W$, then each $T \in \mathscr{L}(V,W)$ has a matrix representation 
$$
\begin{align*}
M(T) = \begin{matrix}
w_{1} \\
\vdots \\
w_{m}
\end{matrix}&\ \begin{pmatrix}
\ \qquad \   \\
\ \vdots\  \\
\ \qquad \ 
\end{pmatrix}  \in \mathbb{F}^{m,n} \\
& \begin{matrix}
\quad v_{1} \cdots v_{n}
\end{matrix}
\end{align*}
$$
So $M: \mathscr{L}(V,W) \to \mathbb{F}^{m,n}$.

#### Theorem
If $\dim V = n$, $\dim W = m$, then $\mathscr{L}(V,W) \simeq \mathbb{F}^{m,n}$.

##### Corollary
$\dim \mathscr{L}(V,W) = (\dim V) ( \dim W)$ if both are finite.

### Products and Quotients

#### Defined [[Product (Vector Spaces)]]

##### Notation
- $V_{1} + \cdots + V_{n} = \sum_{i=1}^{n}V_{i}$ .
- $V_{1} \oplus \cdots \oplus V_{n} = \bigoplus_{i = 1}^n V_{i}$.
- $V_{1} \times \cdots \times V_{n} = \prod_{i=1}^{n}V_{i}$.

##### Proposition
$\prod_{i=1}^{n}V_{i}$ is a vector space.


