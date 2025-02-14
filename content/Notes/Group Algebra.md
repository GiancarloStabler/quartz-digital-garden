#definition #abstract-algebra/ring-theory 

#### Definition
For $R$ commutative ring, $( G,  \cdot )$ finite group, and $G = \{ e=g_{1},g_{2},\ldots, g_{n} \}$ with $x_{e}, x_{g_{2}}, x_{g_{3}},\ldots \in R[G]$. The group algebra $R[G] = \{  r_{e} x_{e} + r_{g_{2}}x_{g_{2}} + \ldots + r_{g_{n}}x_{g_{n}} \mid r_{g_{i}}\in R \}$ is a ring along with the following operations,
- $+$ is "component-wise" -> $\left( \sum_{g\in G} r_{g} x_{g} \right)+ \left(\sum_{g\in G} r'_{g}x_{g}\right) = \sum_{g\in G} (r_{g}+r'_{g})x_{g}$
- $\cdot$ is induced from 
	- distributivity
	- asking $r \in R$, $r = r \cdot x_{e} + \sum_{ g \neq e} 0 x_{g} \in R$ to commute with all $R[G]$
	- $x_{g}x_{h} = x_{gh}$

$R[G]$ has additive identity $0_{R[G]}=0_{R}$.

If $R$ is unital, $R[G]$ is also unital.

$R[G]$ is commutative if and only if $G$ is commutative.

#### Examples


