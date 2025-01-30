#note #analysis/real-analysis 


As we've covered, $\mathbb{Q}$ satisfies the axioms of closure and associativity under addition, multiplication, and the distribution law so it is a [[Field|field]]. Furthermore, $\mathbb{Q}$ satisfies the axiom of order, so it is an ordered field. 

*Goal:* extend $\mathbb{Q}$ in a unique way to $\mathbb{R}$ by adding an additional axiom. 

### The Completeness Axiom

This is the axiom that differentiates the real numbers from the rational numbers.

#### Necessary Definitions
- Defined [[Maximum|maximum]]
- Defined [[Minimum|minimum]]
- Defined [[Supremum|supremum]]
- Defined [[Infimum|infimum]]

#### Writing Proofs with Supremum and Infimum

##### Example
Suppose $S=(-\infty,1) = \{ x\in \mathbb{R} \mid x<1 \}$.

*Claim:* $M=1$ is the supremum of $S$.
###### Proof
We know that $M=1$ is an upper bound of $S$ because for all $x \in S$, $x < 1$.

Suppose that $M'$ is another upper bound of $S$.
*We want to show that $M \leq M'$.*

Assume for the sake of contradiction that $M' < M$, so $M' < 1$. Hence by the definition of $S$, $M' \in S$, so $M'$ is the maximum of $S$. However, we know that $S$ does not have a maximum (suppose $x\in S$ is the maximum of $S$, then we have that $(x+1)/2 \in S$, so $x$ is not the maximum of $S$). Thus a contradiction has been reached and $M \leq M'$.

#### Defined [[The Completeness Axiom]]

Why does the completeness axiom not hold in the rational numbers?
	Suppose we had a set $Q \subset \mathbb{Q}$, defined by $Q= \{ x\in \mathbb{Q} \mid x < \sqrt{ 2 } \}$. We can not identify a supremum for $Q$ because for any $a \in \mathbb{Q}$ that we suppose is the supremum of $Q$, we could find $a' \in \mathbb{Q}$ such that $\sqrt{ 2 } < a' < a$, so $a$ could not be the supremum of $Q$.

#### Defined [[Archimedean Property]]





