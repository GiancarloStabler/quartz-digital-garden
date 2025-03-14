#theorem #abstract-algebra/ring-theory 

#### Formal Definition
Given commutative [[ring]] $(R, +, \cdot)$ with $1_{R}$, and [[ideal]] $I \unlhd R$, there exists a [[Morphism of Rings|morphism]]:
$$
\varphi: R \to S = {^{\textstyle R}\big/_{\textstyle I}}, \quad \varphi(r)=r+I.
$$
where the $\ker \varphi=I$, and $\varphi$ is a surjective morphism.

There are bijective correspondences between:
$$
\{ J \unlhd R \mid I \subseteq J \}\text{, and } \{ a \unlhd S={^{\textstyle R}\big/_{\textstyle I}} \}
$$
#### Proof
We already know from groups, $( {^{\textstyle J}\big/_{\textstyle I}}, + ) \leq ( {^{\textstyle R}\big/_{\textstyle I}}, + )$.

If $x\in J, x+I \in {^{\textstyle J}\big/_{\textstyle I}}$, and if $r \in R, r+I \in {^{\textstyle R}\big/_{\textstyle I}}$. Thus, $(r+I)(x+I)=rx+I \in {^{\textstyle J}\big/_{\textstyle I}}$.

Then, the proof is as for groups.

#### Examples 

