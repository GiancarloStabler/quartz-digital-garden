#definition #abstract-algebra/ring-theory 

#### Definition
For a morphism $f: (R,+,\cdot) \to (S, +, \cdot)$, 
$$
{^{\textstyle R}\big/_{\textstyle \ker f}} \simeq \operatorname{im}f \text{ as rings}.
$$
An isomorphism is $F(r+\ker f)=f(r)$.

#### Proof
Already know from groups that $F$ is a well-defined morphism of additive groups, and an isomorphism of groups (bijective). Hence we know it preserves addition, now it remains to show it preserves multiplication.

$$
\begin{align}
F((r+\ker f)(s + \ker f)) &\overset{?}{=} F(r+\ker f)\cdot F(s + \ker f) \\
f((rs)+\ker f) &\overset{?}{=} f(r) \cdot f(s) \\
f(rs) &= f(rs).
\end{align}
$$



