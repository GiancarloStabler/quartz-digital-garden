#note #abstract-algebra/ring-theory 

#### Defined [[Correspondence Theorem for Quotients]]

Take $(R,+, \cdot)$ a ring with $1_{R}$, and $S = {^{\textstyle R}\big/_{\textstyle I}}$ for some ideal $I \unlhd R$.

##### Remark
Given morphism $f: R \to S$, if $a \unlhd S$, then $f ^{-1} a \unlhd R$. 

##### Remark
If $f: R \to S$ is a morphism, $I \unlhd R$, $f$ not necessarily surjective. Then $f(I) \subseteq S$ is an additive subgroup, but not necessarily an ideal.

##### Remark
If $I \unlhd R$, $I \subseteq J$, $J \unlhd R$, then ${^{\textstyle J}\big/_{\textstyle I}} \unlhd {^{\textstyle R}\big/_{\textstyle I}}$. 

###### Proof
We already know from groups, $( {^{\textstyle J}\big/_{\textstyle I}}, + ) \leq ( {^{\textstyle R}\big/_{\textstyle I}}, + )$.

If $x\in J, x+I \in {^{\textstyle J}\big/_{\textstyle I}}$, and if $r \in R, r+I \in {^{\textstyle R}\big/_{\textstyle I}}$. Thus, $(r+I)(x+I)=rx+I \in {^{\textstyle J}\big/_{\textstyle I}}$.


##### Remark
$I \unlhd R$, $J\unlhd R$ that does not necessarily contain $I$. Then, ${^{\textstyle  J}\big/_{\textstyle I}}$ does not even make sense as additive group, if $I \not \subseteq J$.

**Question:** What is $\varphi(J) \subseteq S = {^{\textstyle R}\big/_{\textstyle I}}$? (Where $\varphi(J)=\{ r+I \mid r \in J \}$, set of cosets in $R$)
**Answer:** It is still an ideal: ${^{\textstyle J+I}\big/_{\textstyle I}}$.

*Note:* $J+I \unlhd R$, $I \subseteq J+I$, so ${^{\textstyle J+I}\big/_{\textstyle I}}\unlhd S={^{\textstyle R}\big/_{\textstyle I}}$. 


##### Example
The image of $10\mathbb{Z}$ in $\mathbb{Z}_{6}$ is 
$$
(10 (\bmod 6)) \underset{10 \equiv 4 \bmod 6}{=} (4) \underset{10 \equiv 4 \bmod 6}{=} (-2) \underset{\text{as ideals}}{=} (2) \unlhd \mathbb{Z}_{6}.
$$
With the previous remark:
We get ${^{\textstyle 10\mathbb{Z}+6\mathbb{Z}}\big/_{\textstyle 6\mathbb{Z}}}=(2) \unlhd \mathbb{Z}_{6}$.

#### Defined [[Units in Rings]]

Given $(R,+, \cdot)$ ring with $1_{R}$. Assume $R$ is commutative.

##### Remark
$u\in R$ is a unit if and only if $((u)=Ru)=((1_{R})=R).$ ($I\in R$, $I = R \iff 1\in I$).

##### Remark 
For any $u\in R$, there exists $\varphi: R\to R$ given by $\varphi(x)= u \cdot x$. $\varphi$ is additive: $\varphi(x+y) = u \cdot (x+y) = ux - uy=\varphi (x) + \varphi(y)$.

The following are equivalent:
- $u$ is a unit.
- $\varphi$ is surjective.
- $\varphi$ is bijective.

In this case, $\varphi ^{-1} = \psi$, with $\psi: R \to R$ defined by $\psi(y) = u ^{-1} y$.

#### Defined [[Zero-Divisor]] and [[Prime Ideal]]

