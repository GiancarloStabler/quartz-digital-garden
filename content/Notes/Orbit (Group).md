---
dg-publish: true
---
#definition #abstract-algebra/group-theory 

#### Definition
The orbit of $x$ with respect to a [[group]] $G$ is the set of all elements equal to the possible actions on $x$ with elements $g\in G$.
$$
\operatorname{orb}(x) = \operatorname{orb}_{G}(x) = \{ g\bullet x : g\in G \}
$$

#### Examples
1) $G=GL_{2}(\mathbb{R})\circlearrowleft \mathbb{R}^2$
	$A \bullet v = Av$
	If $v=\begin{pmatrix}0\\0\end{pmatrix}$
	$\operatorname{orb}(v) = \{ \begin{pmatrix}0\\0\end{pmatrix} : A\begin{pmatrix}0\\0\end{pmatrix} = \begin{pmatrix}0\\0\end{pmatrix}\}$
	We need $A$ invertible, first column is $\begin{pmatrix}a\\b\end{pmatrix}$. For instance, $A=\begin{pmatrix}a & -b \\ b & a\end{pmatrix}$ will work.
	$A^{-1}=\frac{1}{a^2+b^2}\begin{pmatrix}a & b \\ -b & a\end{pmatrix}$ .

2) $G \circlearrowleft G$ by conjugation, 
	$\operatorname{orb}(x) = \{  g\bullet x : g\in G \} = \{  gxg^{-1} : g\in G \}=$ the conjugacy class of $x$ (recall from the class equation).

3) $(\mathbb{Z}_{2}, +)$ acts on the circle $\mathbb{S}1= \bigcirc$
	If $x$ is some point on the circle, then $0\bullet x=x$ and $1 \bullet x =$ the antipodal point on the circle.
	$\operatorname{orb}(x) = \{ 0\bullet x, 1\bullet x \} = \{ x,-x \}$

#### See
- [[Note - Orbits and Stabilizers]]
