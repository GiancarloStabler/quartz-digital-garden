---
dg-publish: true
---
#notes #number-theory/quadratic-integers  

#### Recall: Division Algorithm in $\mathbb{Z}[i]$
For all $\alpha,\beta \in \mathbb{Z}[i]$ such that $\beta \neq 0$, there exists some $\gamma, \rho \in \mathbb{Z}[i]$ such that 
$$
\alpha = \beta \gamma + \rho
$$
where $N(\rho) < N(\beta)$ ([[Norm (Quadratic Integers)|norm]])
#### Recall: Division Algorithm in $\mathbb{Z}[\sqrt{2}]$
1) For all $\alpha,\beta\in \mathbb{Z}[\sqrt{ 2 }]$ such that $\beta\neq_{0}$, there exists some $\gamma,\rho \in \mathbb{Z}[\sqrt{ 2 }]$ such that
$$
\alpha = \beta \gamma + \rho
$$
	where $|N(\rho)| < |N(\beta)|$.

#### To carry this out, we'll use modified division algorithm in $\mathbb{Z}$:
- Usual one: For all $\alpha,\beta \in \mathbb{Z}$ such that $b\neq 0$, for some $q,r \in \mathbb{Z}$ such that $a=bq+r$, $0 \leq r < |b|$.
- Modified one: For all $\alpha,\beta \in \mathbb{Z}$ such that $b\neq 0$, for some $q,r \in \mathbb{Z}$ such that $a=bq+r$, $|r| \leq \frac{1}{2}|b|$. 
	- This allows us to add or subtract up to half of $|b|$ from $bq$, rather than only add up to $|b|$.

#### Examples
1) $\mathbb{Z}[i]:\alpha = 12 +37i, \beta = 7+11i$
$$
\begin{align*}
\frac{\alpha}{\beta} = \frac{{\alpha \bar{\beta}}}{\beta \bar{\beta}} &= \frac{{(12+37i)(7-11i)}}{(7+11i)(7-11i)}\\
&= \frac{491+127i}{170}\\
&\approx 2.88 + 0.74i\\
&\approx 3 + 1i
\end{align*}
$$
$$
\text{Use } \gamma=3+I.
$$
	Set $\rho = \alpha- \beta \gamma = 2-3i$, so $N(\rho)= N(2-3i)=13 < N(\beta)$.

2) $\mathbb{Z}[\sqrt{ 2 }]: \alpha=27+2\sqrt{ 2 }, \beta = 7 + 3\sqrt{ 2 }$
$$
\begin{align*}
\frac{\alpha}{\beta} = \frac{{\alpha \bar{\beta}}}{\beta \bar{\beta}} &= \frac{{(27+2\sqrt{ 2 })(7-3\sqrt{ 2 })}}{(7+3\sqrt{ 2 })(7-3\sqrt{ 2 })}\\
&= \frac{177-67\sqrt{ 2 }}{31}
\end{align*}
$$
$$
\text{{Use }}\gamma = 6-2\sqrt{ 2 }
$$
	Set $\rho = \alpha- \beta \gamma = (-3)^2-2(-1)^2=9-2=7$, so $|N(\rho)|= 7 < N(\beta)$.

#### Remark
See Example 3.2 in $\mathbb{Z}[i]$ notes where $N(\rho)>N(\beta)$ when using nearest integer to the *left* to get $\gamma$.

[[Examples of Euclid's Algorithm in Quadratic Integers]]

### Big Idea
##### In $\mathbb{Z}$,
Division Algorithm 
-> Euclid's Algorithm for GCD
-> Bezout's Identity
-> $p \mid ab$, $p$ prime => $p\mid a$ or $p \mid b$
-> Uniqueness of prime factorization
Separately proved existence of prime factorization (for numbers $\nleq 0$ or $\pm 1$), so we get unique factorization into primes!
##### We have division algorithm in
$F[x]$ for $F$ field
$\mathbb{Z}[i]$
$\mathbb{Z}[\sqrt{ 2 }]$ 
So these *all* have unique factorization into [[Examples of Primes in Quadratic Integers]]!