---
dg-publish: true
---
#proof #number-theory/quadratic-integers/gaussian-integers 

#### Theorem
For all $\alpha,\beta$ in $\mathbb{Z}[i]$ with $\beta \neq 0$, there are $\gamma,\rho$  in $\mathbb{Z}[i]$ such that
$$
\alpha = \beta \gamma + \rho \text{  with  } N(\rho) < N{\beta}\quad \left( \text{in fact, } N(\rho)\leq \frac{1}{2} N(\beta) \right)
$$

#### Proof
Write $\frac{\alpha}{\beta} = \frac{{\alpha \bar{\beta}}}{\beta \bar{\beta}}=\frac{{\alpha \bar{\beta}}}{N(\beta)}=\frac{{m+ni}}{N(\beta)}$ for $m,n \in \mathbb{Z}$

We use [[Note - Modified Division Algorithm|modified division algorithm]] in $\mathbb{Z}$ (least $|r|$) to write in $\mathbb{Z}$
$$
\begin{align*}
m=(N\beta)q_{1}+r_{1} &\qquad |r_{1}| \leq \frac{1}{2} N\beta\\
n=(N\beta)q_{2} + r2 &\qquad |r_{2}| \leq \frac{1}{2}N\beta
\end{align*}
$$
$\implies \alpha \bar{\beta} = m+ni=(N\beta)(q_{1}+q_{2}i)+r_{1}+r_{2}i$

We can call this $\rho=q_{1}+q_{2}i$, and we want to show $N(\rho) \leq \frac{1}{2}N(\beta) < N\beta$

Then $\alpha \bar{\beta} = (N\beta)\gamma + (r_{1}+r_{2}i)$
	$\alpha \bar{\beta}=\beta \bar{\beta}\gamma+r_{1}+r_{2}i$
	$(\alpha-\beta \gamma)\bar{\beta}=r_{1}+r_{2}i$
	$\rho \bar{\beta}=r_{1}+r_{2}i$
	Apply norm:
		$N(\rho)N(\bar{\beta})=r_{1}^2+r_{2}^2 \leq \frac{1}{4} (N\beta)^2+\frac{1}{4}(N\beta)^2$
		$N(\rho)N(\beta) \leq \frac{1}{2}(N(\beta))^2$
		$N(\rho) \leq \frac{1}{2}N(\beta))$ $\qquad \square$

##### Note
If we were to do this in $\mathbb{Z}[\sqrt{ 2 }]$ for example, the proof would be almost the same up to changing $i$ to $\sqrt{ 2 }$, until we reach the "apply the norm" step, in which case we need to use the absolute value of the norms, since the norm can be positive or negative.

#### Remark
For prime $p$ and square-free $d\in \mathbb{Z}$, 
$$
p=x^2-dy^2 \implies p \not\mid y \implies d \equiv \square \bmod p.
$$
"Conversely," if $\mathbb{Z}[\sqrt{ d }]$ has unique factorization:
$$
d\equiv \square \bmod p \implies p \text{ or } -p \text{ is } x^2-dy^2 \text{ in } \mathbb{Z}.
$$
