#note #analysis/real-analysis 

#### Last Time
We proved the [[Bolzano-Weierstrass Theorem]].

If $(x_{n})_{n}$ is bounded, then by Bolzano-Weierstrass, we have that $x_{n_{k}} \to L$ for some subsequence $x_{n_{k}}$. 

However, if $(x_{n})_{n}$ is bounded and monotone, then by the [[Monotone Convergence Theorem]], we have that $x_{n} \to L$. 

#### Example
$$
\begin{cases}
x_{n+1} = 1 + \frac{1}{x_{n}},  \\
x_{1} = 1.
\end{cases}
$$
Guess the limit: 
$L = 1+ \frac{1}{L}$ so $L^2 - L -1 =0$, and $L = \frac{1 \pm \sqrt{ 5 }}{2}$, and thus $L = \frac{1+\sqrt{ 5 }}{2}$ since $x_{n} > 0$.


