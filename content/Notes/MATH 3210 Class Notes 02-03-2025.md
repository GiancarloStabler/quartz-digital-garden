#note #abstract-algebra/vector-spaces 

#### Recall [[Span]] and [[Linear Combination]]

#### Discussed [[Polynomial|Polynomials]] as a Vector Space

#### Proved [[Linear Dependence Lemma]]

##### Theorem

In a [[finite-dimensional]] [[vector space]], the length of every linearly independent list of vectors is less than or equal to the length of every spanning list of vectors.

###### Proof
Suppose $u_{1},\ldots,u_{m} \in V$ is linearly independent and $w_{1},\ldots,w_{m}\in V$ spans $V$. We need to show that $m\leq n$.

Let $B$ be the list $w_{1},\ldots, w_{n}$, which spans $V$. Then the list $u_{1},w_{1},\ldots, w_{n}$ is linearly dependent since $u_{1}\in \operatorname{span}(w_{1},\ldots,w_{n})$ by assumption. By the [[linear dependence lemma]], one of $u_{1},w_{1},\ldots,w_{n}$ is a linear combination of the previous vectors in the list. $u_{1}\neq 0$ since $u_{1},\ldots, u_{m}$ is linearly independent. So $k\neq 1$ in the lemma. Therefore, we can remove some $w_{i}$ from the list, and preserve the span. So $V= \operatorname{span}(u_{1},(n-1) \text{ remaining w's})=B$.

Step $k$, for $k=2,\ldots, m$: 
After step $k-1$, the list $B$ looks like $u_{1},\ldots, u_{k-1}, ((n-k+1)\text{ w's})$. Also $B$ spans $V$. Thus, $u_{k}\in \operatorname{span}(B)$, so $u_{1},\ldots, u_{k-1},u_{k},(n-k+1\text{ w's})$ is linearly dependent.

Since $u_{1},\ldots, u_{k}$ is linearly independent, our index from the linear dependent lemma must "point to" some $w_{i}$. Thus, we can remove this $w$ and preserve the span. 

Since we can do this for all the $u$'s, $m\leq n$.


##### Theorem
Every subspace of a finite-dimensional vector space is finite dimensional.


$$
f(x)= \sum_{n=1}^{\infty} \frac{x^2}{4}+ \pi +4! 
$$
