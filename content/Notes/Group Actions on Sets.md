---
dg-publish: true
---
#definition  #abstract-algebra/group-theory 
#### Definition
Take a [[group]] $( G, \cdot )$, and a set $X$. Assume we have $\mu:G\times X \to X$.

Denote $\mu(g,x)=g\bullet x$ the "action" of $g\in G$ on $x\in X$ such that:
1) $e_{G} \bullet x = x$.
2) Associativity $g\bullet (g'\bullet x) = (gg')\bullet x$.

#### Examples
1) $GL_{2}(\mathbb{R})$ act on $\mathbb{R}^2$ by $A\bullet v = Av$ <- $2\times2$ matrix and $\begin{pmatrix}x\\ y\end{pmatrix}$ column vector.
	$A \bullet v = \begin{pmatrix}a_{11}x + a_{12}y \\ a_{21}x+a_{22}y\end{pmatrix} \leftarrow \mathbb{R}^2$

1) $( S_{n}, \cdot )$ symmetric permutation group acts on $\{ 1,2,\ldots, n \}$ by $\sigma \cdot i = \sigma(i)$ where $\sigma = \begin{pmatrix}1 & 2 & \ldots & n \\ \sigma(1) & \sigma(2) & \ldots & \sigma(n)\end{pmatrix}$

3)  $( G, \cdot )$ group. $G$ acts on itself by left multiplication: $g \bullet g'=gg'$ (note that $\bullet$ is the action and $gg'$ is the product in $G$)

4) $( G, \cdot )$ also acts on $G$ by [[Conjugate (Groups)|conjugation]]: $g\bullet g' \overset{def}{=} gg'g^{-1}$ <- conjugation in $G$. 
	Verification: $\mu(g,g') = gg'g^{-1} \in G$, and $\mu: G\times G \to G$ is well-defined.
	$e_{G} \bullet g' = eg'e^{-1} = g'\ \forall g'\in G$
	$g\bullet(g' \bullet g'') = g\bullet (g'g''(g')^{-1} = gg'g''(g')^{-1}(g'')^{-1} = (gg') g'' (gg')^{-1} = (gg') \bullet g''$.

#### See
- [[Note - Group Actions on Sets]]