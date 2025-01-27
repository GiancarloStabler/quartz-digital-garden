#note #linear-algebra


#### Abstraction
We will take concepts like $\mathbb{R}^n$ and matrices from MATH 2210 and abstract them to abstract vector spaces and linear maps.

#### Review: $\mathbb{R}^n$ and $\mathbb{C}^n$ 
$$
\mathbb{C} = \{  a+bi : i^2=\sqrt{ -1 },\ a,b \in \mathbb{R}\}
$$

We will generally prefer working with $\mathbb{C}^n$ because $\mathbb{C}$ is [[Algebraically Closed Field|algebraically closed]].

We will note a generic field as $\mathbb{F}$, which we can usually think of as $\mathbb{R}$ or $\mathbb{C}$ (and sometimes $\mathbb{F}_{q^n}$, a field of prime order). Generic elements of $\mathbb{F}$ are scalars.

##### Properties of Complex Arithmetic
1) Commutativity
	$\alpha + \beta = \beta + \alpha \quad \forall \alpha,\beta \in \mathbb{C}$ 
	$\alpha \beta = \beta \alpha$ 
2) Associativity
	$\alpha + (\beta + \gamma) = (\alpha + \beta) + \gamma \quad \forall \alpha, \beta, \gamma \in \mathbb{C}$
	$\alpha(\beta \gamma) = (\alpha \beta) \gamma$
3) Identities
	$\alpha + 0 = \alpha \quad \forall \alpha \in \mathbb{C}$
	$1 \alpha = \alpha$
4) Inverses
	For all $\alpha \in \mathbb{C}$, $\exists -\alpha \in \mathbb{C}$ such that $\alpha + (-\alpha) = 0$.
	For all $\alpha \neq 0 \in \mathbb{C}$, $\exists \frac{1}{\alpha} \in \mathbb{C}$ such that $\alpha ( \frac{1}{\alpha})=1$.
5) Distribution 
	$\alpha(\beta + \gamma) = \alpha \beta + \alpha \gamma \quad \forall \alpha, \beta,\gamma \in \mathbb{C}$.


#### Background

*Definition:*
Let $n$ be a positive integer. $\mathbb{F}^n$ is the set of all $n$-tuples of elements of $\mathbb{F}$:
$$
\mathbb{F}^n = \{  (x_{1},x_{2},\ldots,x_{n}) : x_{k} \in \mathbb{F} \text{ for } K=1,\ldots,n\}.
$$
We say $x_{k}$ is the $k$-th coordinate of $(x_{1},\ldots, x_{n})$.

*Definition:*
Addition in $\mathbb{F}^n$ is done component-wise.


#### Proposition:
If $x,y\in \mathbb{F}^n$, then $x+y=y+x$.

##### Proof:
$$
\begin{align}
x+y  & = (x_{1},\ldots, x_{n}) + (y_{1}, \ldots, y_{n}), \\
 & = (x_{1}+y_{1}, \ldots, x_{n} + y_{n}), \\
 & = (y_{1}+x_{1}, \ldots, y_{n} + x_{n}), \\
 & = (y_{1},\ldots, y_{n}) + (x_{1}, \ldots, x_{n}).\\
\end{align}
$$
