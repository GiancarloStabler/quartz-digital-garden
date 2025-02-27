#note #analysis/real-analysis 

## Exam Format

#### Problem 1
1) Compute $\sup, \inf$ of a set.
2) Work with $\sup$, $\inf$ for some set.

*Definition:* $M = \sup S$ if
- $M$ is an upper bound of $S$.
- If $M'$ is another upper bound, then $M' \geq M$.

*Property:* $M = \sup S$ if and only if,
- $M$ upper bound of $S$
- $\forall \varepsilon > 0$, $\exists x \in S$ such that $x \leq M \leq x+ \varepsilon$.

If $(x_{n})_{n}$ is monotonically increasing, then $\sup \left\{ x_{n} : n \right\} = \lim_{ n \to \infty }(x_{n})$ 

#### Problem 2
1) Use $\varepsilon$ definition to calculate the limit of a sequence.
2) Apply the $\varepsilon$ definition to prove properties of sequences (may need to use the triangle inequality). 

#### Problem 3
Apply monotone convergence theorem for a sequence given recursively.
1) Bounded (needs induction)
2) Monotone (needs induction)
3) Limit

$(x_{n})_{n}$ monotonically increasing implies $x_{n} \geq x_{1}$ (lower bound), so only need upper bound.


### Not Tested
1) Set operations ($\cup,\cap,$ DeMorgan's law)
2) Simple induction (like $1+2+\cdots+ n = \frac{n(n+1)}{2}$)
3) Subsequence-related problems (will be on midterm 2).

#### Proving a Sequence is Monotone
$a_{n+1}= f(a_{n})$.
1) Induction
	If $a_{n-1} \leq a_{n}$ prove $a_{n} \leq a_{n+1}$. We have $a_{n} \leq a_{n+1} \iff f(a_{n-1}) \leq f(a_{n})$.
2) Check directly
	$a_{n+1} \geq a_{n} \iff f(a_{n}) \geq a_{n}$ and solve in $a_{n}$.

#### Common Mistakes
1) A sequence being convergent does *NOT* necessarily imply that the sequence is monotone.