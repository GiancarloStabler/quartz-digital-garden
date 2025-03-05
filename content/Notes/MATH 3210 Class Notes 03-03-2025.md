#note #abstract-algebra/vector-spaces 

## Duality

### [[Dual Vector Space]]
Defined the dual vector space, dual basis, and dual transformation.

##### Example 1
Let $D \in \mathscr{L}(P(\mathbb{R}), P(\mathbb{R}))$ be differentiation. How does $D'$ behave?
1) Pick $\varphi(p)= p(3) \in W'=(P(\mathbb{R}))'$.
	$D'(\varphi) = \varphi \circ D \implies D'(\varphi)(p)=p'(3)$.
2) $\varphi(p) = \int_{0}^1p \in (P(\mathbb{R}))'$.
	$D'(\varphi)(p)=(\varphi \circ D)(p) = \int_{0}^1p'=p(1)-p(0)$.

##### Theorem 1
Suppose $T \in \mathscr{L}(V,W)$. Then,
1) $(S+T)' = S'+ T'$ for all $S \in \mathscr{L}(V,W)$.
2) $(\lambda T)' = \lambda T'$.
3) $(ST)'=T'S'$ for all $S \in \mathscr{L}(W,U)$.

### Null Space and Range of Dual Maps

#### Defined the [[Annihilator]]

##### Example 2
Let $U \subseteq P(\mathbb{R})$ be all the multiples of $x^2$. What's an example of $\varphi \in U^0$?

$\varphi(p)=p'(0) \in U^0$. 

##### Recall [[Fundamental Theorem of Linear Maps]]

##### Example 3
Let $e_{1},e_{2},e_{3},e_{4},e_{5}$ be the standard basis of $\mathbb{R}^5$; let $\varphi_{1},\ldots, \varphi_{5}$ be the dual basis in $(\mathbb{R}^5)'$ (note $\varphi_{j}(x_{1},\ldots,x_{5})=x_{j}$).

Suppose $U = \operatorname{span}(e_{1},e_{2})=\left\{ (x_{1},x_{2},0,0,0) \subseteq \mathbb{R}^5 \right\}$.

What is $U^0$? Claim: $U^0=\operatorname{span}(\varphi_{3},\varphi_{4},\varphi_{5})$.

#### Theorem 2
If $U \subseteq V$, then $U^0$ is a [[subspace]] of $V'$.

##### Proof
1) $0$ is in $V'$ and $U^0$.
2) $\varphi_{1},\varphi_{2} \in U^0$, then $(\varphi_{1}+\varphi_{2})(u) = \varphi_{1}(u) + \varphi_{2}(u)= 0$, so $\varphi_{1}+\varphi_{2} \in U^0$.
3) $\lambda \varphi_{1} \in U^0$.

Thus, $U^0$ is a subspace of $V'$.

#### Theorem 3
Suppose $V$ is finite-dimensional and $U$ is a subspace of $V$, then
$$
\dim U^0 = \dim V - \dim U.
$$

##### Proof
1) Take a basis of $U$: $u_{1},\ldots, u_{m}$, extend to a basis of $V$: $u_{1},\ldots,u_{m},\ldots,u_{n}$. Then show $\varphi_{m+1},\ldots, \varphi_{n}$ is a basis of $U^0$.
2) Let $i \in \mathscr{L}(U,V)$ be the inclusion map ($i(u) = u \in V$). Thus, $i' \in \mathscr{L}(V',U')$. The FTLM implies that $\dim \operatorname{range}(i') + \dim \operatorname{null} (i') = \dim V'$. However, $\operatorname{null}(i') = U^0 = \left\{  \varphi \in V' : \varphi \circ i = 0 \text{ on } U \right\}$, and $\dim V' = \dim V$, so $\dim\operatorname{range}i' + \dim U^0 = \dim V$. If $\varphi \in U^0$, then $\varphi$ can be extended to a linear functional $\psi$ on $V$. Then the definition of $i'$ shows $i'(\psi) = \varphi = \psi \circ i$. Thus, $\varphi \in \operatorname{range}i'$, so $\operatorname{range}i' = U'$. So, $\dim \operatorname{range}i' = \dim U' = \dim U$.

With 1) and 2) together, we have $\dim U^0 = \dim V -\dim U$.

#### Theorem 4
Suppose $V,W$ are finite-dimensional and $T \in \mathscr{L}(V,W)$, then
1) $\operatorname{null}(T')=(\operatorname{range}(T))^0$.
2) $\dim\operatorname{null}(T') = \dim \operatorname{null}(T) + \dim W - \dim V$.

##### Proof
In the book.

##### Corollary
Suppose $V,W$ are finite-dimensional and $T \in \mathscr{L}(V,W)$, then $T$ is [[surjective]] if and only if $T'$ is [[injective]].

#### Theorem 5
Suppose $V,W$ are finite=dimensional and $T \in \mathscr{L}(V,W)$. Then,
1) $\dim \operatorname{range}(T') = \dim \operatorname{range}(T)$.
2) $\operatorname{range}(T') = (\operatorname{null}T)^0$.

##### Corollary
Suppose $V,W$ are finite-dimensional and $T \in \mathscr{L}(V,W)$, then $T$ is injective if and only if $T'$ is surjective.

#### Theorem 6
Suppose $V,W$ are finite-dimensional and $T\in \mathscr{L}(V,W)$, then the matrix $M(T') = M(T)^t$ (transpose).