#definition #abstract-algebra/vector-spaces 

#### Definition
Given a [[vector space]] $V$, we have $V' = \mathscr{L}(V, \mathbb{F})$ is the dual space. 

#### Dual Basis
Given a basis $v_{1},\ldots, v_{n}$ of $V$, we can form the dual basis, $\varphi_{1},\ldots,\varphi_{n} \in V'$ defined by,
$$
\varphi_{j}(v_{k}) = \begin{cases}
1 & j = k  \\
0 & j \neq k
\end{cases}
$$
The elements $\varphi_{j}$ are a basis of $V'$ if $V$ is [[finite-dimensional]].

#### Dual Transformation
Given a [[linear map]] $T \in \mathscr{L}(V,W)$, the dual of $T$ is $T' \in \mathscr{L}(W',V')$ defined by $T'(\varphi) = \varphi \circ T$ for $\varphi \in W'$.

#### Examples


