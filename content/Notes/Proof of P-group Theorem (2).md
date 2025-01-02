---
dg-publish: true
---
#proof #abstract-algebra/group-theory/p-groups 
#### Theorem
For [[P-group|p-group]] $( G, \cdot )$, $p$ prime such that $|G| = p^k$. Then there exist unique integers $f_{1}\geq f_{2} \geq \ldots \geq f_{a} \geq 1$ such that $f_{1}+f_{2}+\ldots + f_{a}=k$, and $G \simeq \mathbb{Z}_{p}f_{1} \times \ldots \mathbb{Z}_{p}f_{a}$.

#### Proof
*Strategy:* construct elements
$g_{1},\ldots, g_{a}\in G$ such that $g_{1}$ has the largest possible order $p^{f_{1}}$ among all group elements.
$g_{2} \cdot \langle g_{1} \rangle$ has largest possible order $p^{f_{2}}$ in ${^{\textstyle G}\big/_{\textstyle \langle g_{1} \rangle}}$.
$g_{3} \cdot \langle g_{1},g_{2} \rangle$ has largest order $p^{f_{3}}$ in ${^{\textstyle G}\big/_{\textstyle \langle g_{1},g_{2} \rangle}}$ and so on.

Show that up to twisting $g_{i}$ by $g_{1}, \ldots, g{i-1}$, we may assure $\operatorname{ord}_{}(g_{i})=p^{f_{i}}$ in $G$ and $\langle g_{1} \rangle, \langle g_{2} \rangle, \langle g_{3} \rangle, \ldots, \langle g_{a} \rangle$ give an internal direct product decomposition

$\implies G \simeq \langle g_{1} \rangle\times \ldots \langle  g_{a} \rangle$ (note that $\langle g_{1} \rangle=\mathbb{Z}_{p^{f_{1}}}$, and $\langle g_{a} \rangle= \mathbb{Z}_{p^{f_{a}}}$.)


We do first two steps:

Let $g_{i}\in G$ have largest possible order $p^{f_{1}}$.
$g_{2} \in G$ have largest possible order $p^{f_{2}} \bmod \langle g_{1} \rangle$.

If $p^{f_{1}} = p^k = |G| \implies G = \langle g_{1} \rangle \simeq \mathbb{Z}_{p^{f_{1}}}$.

In this case, $a=1$, $f_{1}=k$. 

Let $\pi: G \to {^{\textstyle G}\big/_{\textstyle \langle g_{1} \rangle}}$ (the quotient group is commutative)
$\pi(x) = x \cdot \langle g_{1} \rangle$

*Remark:*
1) ${^{\textstyle G}\big/_{\textstyle \langle g_{1} \rangle}}$ is also a p-group. (This is by Lagrange's Theorem)
2) $x\in G$, $\operatorname{ord}_{G}(x)=p^b\implies \operatorname{ord}_{{^{\textstyle G}\big/_{\textstyle \langle g_{1} \rangle}}}(x\cdot \langle g_{1} \rangle)=p^{b'}$ for some $b' \leq b$. (Note that $x\cdot \langle g_{1} \rangle=\pi(x)$)

$\operatorname{ord}_{{^{\textstyle G}\big/_{\textstyle \langle g_{1} \rangle}}}(\pi(x)) \mid \operatorname{ord}_{G}(x)$

Let $p^{f_{2}} = \operatorname{ord}_{{^{\textstyle G}\big/_{\textstyle \langle  g_{1} \rangle}}}(g_{2} \cdot \langle g_{1} \rangle)$
By the remark above, we have that $\operatorname{ord}_{G}(g_{2})=p^{c}$ for some $c\geq f_{2}$.

Claim: $\exists i \in \mathbb{Z}$,  $g_{2}' = g_{2} \cdot g_{1}^i$ has order $p^{f_{2}}$ in $G$, and still $\operatorname{ord}_{{^{\textstyle G}\big/_{\textstyle \langle g_{1} \rangle}}}(g_{2}'\cdot \langle g_{1} \rangle) = p^{f_{2}} = \operatorname{ord}_{{^{\textstyle G}\big/_{\textstyle \langle g_{1} \rangle}}}(g_{2}\cdot \langle g_{1} \rangle)$.

In this case we will observe that $\langle g_{1} \rangle\cap \langle g_{2}' \rangle= \{ e_{G} \}$.

*Question:* Where does this come from?

#### Examples
$G=(\mathbb{Z}_{4}\times \mathbb{Z}_{2}, +)$

$g_{1}=(1,0)$ has order $4$, largest possible

$g_{2}=(1,1) \in G$ has order $4$, but $g_{2}+\langle g_{1} \rangle$ has order $2$.

#### Remark
Group $( G, \cdot )$, with normal subgroup $N \unlhd G$, $g\in G$, and surjective morphism $\pi: G \to {^{\textstyle G}\big/_{\textstyle N}}$
	$\implies \operatorname{ord}_{{^{\textstyle G}\big/_{\textstyle N}}}(\pi(g))= \operatorname{ord}_{{^{\textstyle G}\big/_{\textstyle N}}}(gN)=$ smallest $n\geq 1$ such that $g^n \in N$ ($\iff g^nN = N$, and $(gN)^n = e_{{^{\textstyle G}\big/_{\textstyle N}}}$).

$\langle g_{1} \rangle= \{ (0,0),(1,0),(2,0),(3,0) \}$
$\langle g_{2} \rangle=\{ (0,0), (1,1), (2,0), (3,1) \}$

Thus, $\langle g_{1} \rangle,\langle g_{2} \rangle$ intersect non-trivially, and can therefore not give an internal direct product decomposition.

But, if we replace $g_{2}$ by $g_{2}-g_{1}=g_{2}'$, now we get $\operatorname{ord}_{G}(g_{2}')=2=\operatorname{ord}_{{^{\textstyle G}\big/_{\textstyle \langle g_{1} \rangle}}}(g_{2}' + \langle g_{1} \rangle)$ (note $g_{2}'+\langle g_{1} \rangle=g_{2}+\langle g_{1} \rangle$)

Therefore, $\langle g_{1} \rangle$ and $\langle g_{2}' \rangle$ do give an internal direct product decomposition.


#### Proof of $\langle g_{1} \rangle\cap \langle g_{2}' \rangle= \{ e_{G} \}$.
Assume $\operatorname{ord}_{}(g_{2})=c > f_{2} = \operatorname{ord}_{{^{\textstyle G}\big/_{\textstyle \langle g_{1} \rangle}}}(g_{2}\langle g_{1} \rangle)$
$\implies \langle g_{1} \rangle \cap \langle  g_{2} \rangle = \langle g_{2}^{p^{f_{2}}} \rangle$

$\operatorname{ord}_{}({^{\textstyle p^c}\big/_{\textstyle p^{f_{2}}}})=p^{c_{0-f_{2}}}$

$\implies$ in $\langle g_{1} \rangle$ this must be $\langle g_{1}^{f_{1}-(c-f_{2})} \rangle$

$\implies g$

