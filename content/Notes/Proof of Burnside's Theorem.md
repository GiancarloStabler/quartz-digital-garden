---
dg-publish: true
---
#proof #abstract-algebra/group-theory 

#### Theorem
The number of distinct orbits of _____ is equal to,
$$
\# orbits = \frac{1}{|G|} \sum_{g\in G}^{}|\operatorname{fix}_{x}(g)|.
$$

#### Proof
Let $I= \{ (g,x) \in G\times X : g \bullet x = x \}$.
$$
\begin{align*}
\# I &= \sum_{g\in G}^{}|\operatorname{fix}_{x}(g)|\\
&= \sum_{ x\in X}^{} |\operatorname{stab}_{G}(x)|
\end{align*}
$$
$\frac{1}{|G|} \sum_{g\in G}^{} |\operatorname{fix}_{x}(g)|=\frac{1}{|G|} \sum_{x\in X}^{}|\operatorname{stab}_{G}(x)|$.

If $x'\in \operatorname{orb}(x) \implies x'=g\bullet x$ for some $g\in G \implies \operatorname{stab}(x') = g \cdot \operatorname{stab}(x) \cdot g^{-1}$.
$h\cdot x = x \implies (hg^{-1}g)\cdot x = x$
$(hg^{-1})\bullet (g\cdot x) = x$
$(ghg^{-1})\bullet (g\cdot x)=g \bullet x$
$\implies |\operatorname{stab}(x')|=|\operatorname{stab}(x)|$

Then rearranging $X$ by orbits, 
$\sum_{x\in X}^{}|\operatorname{stab}_{G}(x)| = \sum_{\text{distinct orbits}}^{}\sum_{x \in \text{ such orbit}}^{} |\operatorname{stab}(x)|$
$= \sum_{\text{distinct orbits}}^{}|G| = \#\text{ distinct orbits}$