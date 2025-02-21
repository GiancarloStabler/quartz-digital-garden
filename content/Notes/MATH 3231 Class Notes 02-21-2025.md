#note #abstract-algebra/ring-theory #abstract-algebra/vector-spaces 

### [[Vector Space|Vector Spaces]]

#### Defined [[Support]]

#### Defined [[Linear Map]]

#### Defined [[Linear Isomorphism]]

#### [[Theorem - Every Vector Space has a Basis]]

#### Theorem
If there exists a vector space $V$ over $k$, with bases $\mathscr{B}= (v_{i})_{i \in I}$ and $\mathscr{C}= (w_{j})_{j \in J}$, then there exists a bijection $f: I \to J$.

##### Corollary
$\dim_{k} V \overset{def}{=}$ the cardinality of any basis of $V$.

#### Definition
For a vector space $V$ with basis $\mathscr{B}=(v_{i})_{i \in I}$, we get $T: k^{\oplus I} \to V$ induced isomorphism, and we define $[v]_{\mathscr{B}} \overset{def}{=} T^{-1}(v)$, the coordinates of $v$ with respect to $\mathscr{B}$.

#### Definition
If $T:V\to V$ a linear operator, and $\mathscr{B}=(v_{i})_{i \in I}$ is a basis, where $\# I = n$, then there exists a unique $n \times n$ matrix $[T]_{\mathscr{B}} = [T]_{\mathscr{B}} \cdot [v]_{\mathscr{B}}$, defined by,
$$
[T]_{\mathscr{B}} = \begin{bmatrix}
\vdots & & \vdots  \\
[T(v_{1})_{\mathscr{B}} & \cdots & [T(v_{n})]_{\mathscr{B}}]  \\
\vdots & & \vdots
\end{bmatrix}.
$$

#### Definition 
$T:V \to V$ a linear operator. $P(x) \in k[x]$ with $P(x) = a_{n} x^n+ \cdots + a_{0}$. We can define $P(T):V\to V$ a linear operator given by
$$
P(T) =a_{n}T^n + \cdots + a_{1}T + a_{j}\cdot I_{v}
$$
Where $I_{v}$ is the identity function such that $I_{v}(v)=v$ for all $v\in V$.

#### Defined [[Characteristic Polynomial]]

#### Remark
If $\dim V =n$ and $\mathscr{B} = v_{1},\ldots, v_{n}$ and $\mathscr{C}=w_{1},\ldots, w_{n}$ are bases of $V$, and $T$ is a linear operator on $V$, then $[T]_{\mathscr{B}},[T]_{\mathscr{C}}$ are "[[Similar Matrices|similar]]" matrices.

#### Remark
For a linear operator $T$ on $V$, where $\dim V = n$,
$$
k[x] \overset{\phi}{\rightarrow} \operatorname{end}_{k}(V)
$$
A morphism of rings, also a linear transformation with
$$
P(x) \mapsto P(T) \text{ as before}
$$
