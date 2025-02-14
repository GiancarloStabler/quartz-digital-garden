#note #analysis/real-analysis 

### Defined [[Limit]]

#### Example
Prove that,
$$
\lim_{ n \to \infty } \frac{n}{2n+1}=\frac{1}{2}.
$$

##### Proof
We want to show that $\forall \varepsilon >0$, $\exists N > 0$ such that $\mid \frac{n}{2n+1} - \frac{1}{2}\mid < \varepsilon$ for all $n > N$.

$$
\begin{align*}
\left\lvert \frac{n}{2n+1} \right\rvert = \left\lvert \frac{{2n-(2n+1)}}{2(2n+1)} \right\rvert = \frac{1}{2(2n+1)} < \frac{1}{n} < \varepsilon \iff n>\frac{1}{\varepsilon}.
\end{align*}
$$

#### Defined [[Triangle Inequality]]

#### Proposition
If the limit of $x_{n}$ exists, then it is unique!

#### Defined [[Increasing (Sequence)]], [[Decreasing (Sequence)]], and [[Monotone (Sequence)]]