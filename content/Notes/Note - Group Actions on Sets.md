---
dg-publish: true
---
#note #abstract-algebra/group-theory 

 [[Group Actions on Sets]]
#### Examples
1) $GL_{2}(\mathbb{R})$ act on $\mathbb{R}^2$ by $A\bullet v = Av$ <- $2\times2$ matrix and $\begin{pmatrix}x\\ y\end{pmatrix}$ column vector.
	$A \cdot v = \begin{pmatrix}a_{11}x + a_{12}y \\ a_{21}x+a_{22}y\end{pmatrix} \leftarrow \mathbb{R}^2$

1) $( S_{n}, \cdot )$ symmetric permutation group acts on $\{ 1,2,\ldots, n \}$ by $\sigma \cdot i = \sigma(i)$ where $\sigma = \begin{pmatrix}1 & 2 & \ldots & n \\ \sigma(1) & \sigma(2) & \ldots & \sigma(n)\end{pmatrix}$

3)  $( G, \cdot )$ group. $G$ acts on itself by left multiplication: $g \bullet g'=gg'$ (note that $\bullet$ is the action and $gg'$ is the product in $G$)

4) $( G, \cdot )$ also acts on $G$ by conjugation: $g\bullet g' \overset{def}{=} gg'g^{-1}$ <- conjugation in $G$. 
	Verification: $\mu(g,g') = gg'g^{-1} \in G$, and $\mu: G\times G \to G$ is well-defined.
	$e_{G} \bullet g' = eg'e^{-1} = g'\ \forall g'\in G$
	$g\bullet(g' \bullet g'') = g\bullet (g'g''(g')^{-1} = gg'g''(g')^{-1}(g'')^{-1} = (gg') g'' (gg')^{-1} = (gg') \bullet g''$.

#### Remark
Say $X$ is a finite set $X=\{  x_{1},\ldots, x_{n} \}$.
$\operatorname{Perm}(X) = \{ f:X\to X : f \text{ bijection} \}$
$(\operatorname{Perm}(X), \circ)$ is a group.

$\operatorname{Perm}(X) \simeq S_{n}$
$f:X\to X \mapsto \sigma$
$f(x_{i}) = x_{\sigma(i)}$ for some permutation of $\{ 1,\ldots, n \}$


If $( G, \cdot )$ is a group, then an action of $G$ on $X$ is the same as a morphism $M:G\to \operatorname{Perm}(X)$.

If $M:G\to \operatorname{Perm}(X)$ is a morphism, we define $\mu:G\times X \to X$ as $\mu(g,x)=M(g)(x)$ <- This is the $M(g)$ permutation on $X$ applied to $x\in X$.

Conversely, from an action $\mu:G\times X \to X$, we observe that for all $g\in G$, $\varphi_{g}:X\to X$ defined by $\varphi_{g}(x) = \mu(g,x) = g\bullet x$, $\varphi_{g}$ is a bijection, so $(\varphi_{g})^{-1} = \varphi_{g^{-1}}$

Define $M:G\to \operatorname{Perm}(X)$ as $M(g) = \varphi_{g}\in \operatorname{Perm}(X)$. $M$ is a morphism. 

##### Proof ($M$ is a morphism)
$M(gg') \overset{?}{=} M(g) \circ M(g')$
$\varphi_{gg'} \overset{?}{=} \varphi_{g} \circ \varphi_{g'}$
$\varphi_{gg'}(x) \overset{?}{=} \varphi_{g}(\varphi_{g'}(x))=\varphi_{g}(g' \bullet x) = g\bullet (g' \bullet x) = (gg')\bullet x=\varphi_{gg'}(x). \qquad \square$


#### Remark
If $G$ acts on $X$, $g^{-1} \bullet (g \bullet x) = (g^{-1}g)\bullet x = e_{G}\bullet x = x$.

##### Example
$D_{4}$ acts on square by rigid motions: rotations and reflections. 

Take $\tau \in D_{4}$ a reflection so $\tau,\tau^{-1}$.

$\tau \bullet (\tau \bullet x) = x$  ($\tau\bullet x$ reflects $x$ across axis of symmetry on $\tau$)
