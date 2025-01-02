---
dg-publish: true
---
#note #abstract-algebra/group-theory 

For finite group $( G, \cdot )$ with $|G| < \infty$.
- If $|G| = p$ prime, then $G$ is cyclic, and $G \simeq ( \mathbb{Z}_{p}, + )$.
- [[Lagrange's Theorem|Lagrange]]: If $H \leq G$, then $|G|=|H| \cdot [G:H]$ $\leftarrow$ $\#$ of left cosets of $H$ in $G$.
- Class Equation: $|G| = |Z(G)| + \sum_{i=1}^{r} \frac{{|G|}}{|Z(x_{i})|}$ 
	$Z(G)$ is the center of $G$, $x_{1},\ldots, x_{r}$ are one element from each distinct conjugacy class with more than one element.
- [[Cauchy's Theorem|Cauchy]]: If $p\geq 2$ prime and $p \mid |G|$, then there exists $x\in G$ such that $\operatorname{ord}_{G}(x)=p$.
- If $|G|=p^2$ and $p$ prime, then $( G, \cdot )$ is commutative.
- [[Note - Structure of Finite Commutative Groups|Structure Theorem for Finite Commutative Groups]]: If $( G, \cdot )$ commutative and finite, then $G \simeq$ product of cyclic [[P-group|p-groups]] $(\mathbb{Z}_{p^k},+)$ for prime $p$ and $k\geq 1$.
- If $N \unlhd G$, $( {^{\textstyle G}\big/_{\textstyle N}}, \cdot )$ is a finite group with $[G:N] = \frac{|G|}{|N|}$ elements.
- If $G$ is a p-group, then $Z(G) \not= \{ e \}$ (also p-group).
- If ${^{\textstyle G}\big/_{\textstyle Z(G)}}$ is cyclic, then ${^{\textstyle G}\big/_{\textstyle Z(G)}}=\{ e \}$, $G=Z(G)$ and $G$ is commutative.
- If $g^2=e\ \forall g\in G$, then $G$ is a commutative 2-group.
	Ex: [[Note - Structure of Finite Commutative Groups|groups with n elements]].
	- $n=1$: $G=\{  e \}$.
	- $n=2$: $G= \mathbb{Z}_{2}$.
	- $n=3$: $G= \mathbb{Z}_{3}$.
	- $n=4$: $G=\mathbb{Z}_{4}$ or $G \simeq \mathbb{Z}_{2} \times \mathbb{Z}_{2}$.
	- ...
- [[Sylow Theorems]] 