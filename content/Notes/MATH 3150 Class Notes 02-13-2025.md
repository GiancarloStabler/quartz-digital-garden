#note #analysis/real-analysis 

#### Recall
For $L\in \mathbb{R}$, $\lim_{ n \to \infty } x_{n}=L$ if $\forall\varepsilon > 0$, there exists $N >0$ so that $\left\lvert x+n - L \right\rvert < \varepsilon$, for all $n > N$.

### [[Monotone Convergence Theorem]]

#### Example
Let
$$
\begin{cases}
x_{n+1} = \sqrt{ 2 +x_{n} }, \\
x_{1} = \sqrt{ 2 }.
\end{cases}, n \geq 1.
$$
##### Prove $\lim_{ n \to \infty }x_{n}=2$.

*Prove the Necessary Conditions are Satisfied:*

Show $(x_{n})_{n}$ is increasing. 

*Method 1:*
1) $x_{n} \leq x_{n+1}$ if and only if $\sqrt{ 2+x_{n-1} } \leq \sqrt{ 2 +x_{n} }$. Square both sides to get $2+x_{n-1} \leq 2+x_{n}$, so $x_{n-1} \leq x_{n}$.
2) Assume that $x_{n-1} \leq x_{n}$, then we have $x_{n} \leq x_{n+1}$, and since $\sqrt{ 2 } \leq \sqrt{ 2 + \sqrt{ 2 } }$, by induction we have that $(x_{n})_{n}$ is increasing.

*Method 2:*
1) $x_{n} \leq x_{n+1}$ if and only if $x_{n} \leq \sqrt{ 2 + x_{n} }$. Square both sides to get, $x_{n}^2 \leq 2 + x_{n}$, which is equivalent to $x_{n}^2 -x_{n}-2 \leq 0 \iff (x_{n}+1)(x_{n}-2) \leq 0 \iff -1 \leq x_{n} \leq 2$.
2) Since we already know that $x_{n} > 0$, we just need to show that $x_{n}\leq 2$. (Side note: this method may seem much more cumbersome, but we will need to show the sequence is bounded later, so this achieves the proof of both necessary conditions at the same time).
	1) $x_{1}=\sqrt{ 2 }\leq 2$.
	2) Assume $x_{n} \leq 2$, then $x_{n+1}=\sqrt{ 2 + x_{n} }\leq \sqrt{ 2 + 2 } = 2$.
	3) Therefore, $x_{n}\leq 2$.

Now we must show $(x_{n})_{n}$ is bounded. By method 2 we've shown that the sequence is bounded ($0\leq x_{n}\leq 2$), if we proceeded by method 1, then we must now show that $(x_{n})_{n}$ is bounded.

So far: $(x_{n})_{n}$ is monotone and bounded, so by the monotone convergence theorem, we have that there exists $L\in \mathbb{R}$ such that $\lim_{ n \to \infty } x_{n} = L$.

Why $L=2$:
$x_{n+1}=\sqrt{ 2+x_{n} } \implies (x_{n+1})^2 = 2 +x_{n}$.
Facts:
1) If $\lim_{ n \to \infty }x_{n}=L \implies \lim_{ n \to \infty }x_{n+1}$. Thus, $\left\lvert x_{n}-L \right\rvert< \varepsilon \ \forall n > N\implies \left\lvert x_{n+1}-L \right\rvert < \varepsilon \ \forall n > N-1$.
2) If $\lim_{ n \to \infty }x_{n}=L_{1}$, and $\lim_{ n \to \infty }y_{n}=L_{2}$, then $\lim_{ n \to \infty }x_{n}y_{n}=L_{1}L_{2}$, so in particular, $\lim_{ n \to \infty }(x_{n})^2=L^2$.
	1) This will be proved next class.

$(x_{n+1})^2 =2 +x_{n}$, so $\lim_{ n \to \infty }(x_{n+1})^2=2+ \lim_{  n \to \infty }x_{n}$, so $L^2=2+L$. We can solve this to get $L=-1$ and $L=2$, of which we can discard $L=-1$ because $L \geq 0$. $\qquad\qquad \square$


### [[Infinite Limit]]

#### Example

$\lim_{ n \to \infty } \frac{n^4 -5n^3}{n + \sqrt{ n }+1}=\infty$.

We need to show that $\frac{n^4 -5n^3}{n+\sqrt{ n }+1} > M$, for all $n > N$.


