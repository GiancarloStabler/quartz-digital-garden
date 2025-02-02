#note #analysis/real-analysis 

Going back to the [[Archimedean Property]]

### How to Prove $M$ is a Supremum

For more abstract proofs we can prove $M$ is a supremum of $S$ by showing that 
1) $M$ is an upper bound of $S$.
2) If $\bar{M}$ is another upper bound of $S$, then $\bar{M} \geq M$.

For more concrete examples, we can instead show,
1) $M$ is an upper bound of $S$.
2) $\forall \varepsilon >0, \exists x \in S$ such that $x \leq M \leq x + \varepsilon$.

#### Proof Examples

##### Proof
"$\implies$"
Prove that if $M=\sup S$, then $\forall \varepsilon > 0, \exists x\in S$ so that $x \leq M \leq x + \varepsilon$.

If $\bar{M}<M$ then $\bar{M}$ is NOT an upper bound of $S$ $\implies \exists x\in S$ so that $\bar{M} < x$.

Apply this for $\bar{M} = M -\varepsilon < M \implies \exists x \in S$ so that $\bar{M} <x$ i.e. $M-\varepsilon < x \implies M < x + \varepsilon$.


"$\impliedby$"
We know $M$ is an upper bound and $\forall \varepsilon > 0, \exists x \in S$ such that $x \leq M \leq x + \varepsilon$.

We want to show that if $\bar{M}$ is an upper bond of $S$ then $\bar{M} \geq M$.

So let $\bar{M}$ be an upper bound of $S$, so $\bar{M} \geq x\quad \forall x \in S$. Since $M \leq x + \varepsilon$ and $x \leq \bar{M}$, we have $M \leq \bar{M} + \varepsilon \quad \forall \varepsilon > 0$. Thus, $M \leq \bar{M}$.