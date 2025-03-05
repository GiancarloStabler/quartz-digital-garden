#note #analysis/real-analysis 

### [[Cauchy Sequence]]

#### Proposition 1
If $(x_{n})_{n}$ convergent, then $(x_{n})_{n}$ is Cauchy.

#### Proposition 2
If $(x_{n})_{n}$ is Cauchy, then $(x_{n})_{n}$ is convergent.

##### Proof
**(Step 1)** $(x_{n})_{n}$ Cauchy $\implies$ $(x_{n})_{n}$ bounded.

We know $\forall \varepsilon >0$, $\exists N > 0$ such that $\left\lvert x_{n} -x_{m} \right\rvert < \varepsilon$, $\forall n,m > N$. From this we can fix $m > N$, and we get $x_{m} - \varepsilon < x_{n} < x_{m} + \varepsilon$. We can define $M_{1} = x_{m} + \varepsilon$, and $M_{2} = x_{m} - \varepsilon$, neither of which depend on $n$, which gives us $M_{2} < x_{n} < M_{1}$ for all $n > N$. Thus $x_{n}$ is bounded.

**(Step 2)** $(x_{n})_{n}$ Cauchy $\implies$ $(x_{n})_{n}$ convergent.

We know,
1) $\forall \varepsilon >0$, $\exists N>0$ such that $\left\lvert x_{n}-x_{m} \right\rvert< \varepsilon$ for any $n,m > N$.
2) $(x_{n})_{n}$ is bounded (proved in step 1).

By the [[Bolzano-Weierstrass Theorem]], from 2), we have $\exists (x_{n_{k}})_{k}$ subsequence that converges to some limit $L$. Hence, $\forall \varepsilon > 0$, $\exists N_{1}>0$ such that $\left\lvert x_{n_{k}} - L \right\rvert < \varepsilon$, $\forall k > N_{1}$.

We need to show $\left\lvert x_{n} - L \right\rvert < \varepsilon$.

We can take $k > N_{k}$ large enough so that $n_{k} > N$, so we can take $m = n_{k} > N$ and get $\left\lvert x_{n}-x_{n_{k}} \right\rvert < \varepsilon$ by 1). Thus,
$$
\left\lvert x_{n}-L \right\rvert = \left\lvert (x_{n}-x_{n_{k}}) + (x_{n_{k}}-L) \right\rvert  \leq \left\lvert x_{n}-x_{n_{k}} \right\rvert + \left\lvert x_{n_{k}}-L \right\rvert < \varepsilon + \varepsilon = 2 \varepsilon,
$$
and we have that $(x_{n})_{n}$ is convergent.

### Applications to Series

#### Recall
We say $\sum_{n=1}^{\infty} x_{n}$ converges if the sequence $S_{n}=x_{1}+ \cdots + x_{n}$ converges as $n \to \infty$.

For most series that are convergent, we are not able to find their sum.

#### When Do We Know a Series Converges
A series $\sum_{n=1}^{\infty}x_{n}$ converges,
1) If all $x_{n} \geq 0$ then $\sum_{n-1}^{\infty}x_{n}$ converges if and only if $\sum_{n=1}^{\infty}x_{n} < \infty$ (i.e. $S_{n}$ is bounded).
2) What if $x_{n}$s do not have a sign?
	If $\sum_{n=1}^{\infty} x_{n}$ is [[Absolute Convergence|absolutely convergent]], then $\sum_{n=1}^{\infty}x_{n}$ is convergent.