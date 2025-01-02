---
dg-publish: true
---
#proof #number-theory/quadratic-integers 

#### Theorem
For any prime $p$,
$$
-1 \equiv \square \bmod p \iff p = x^2+y^2 \text{ in } \mathbb{Z}.
$$

#### Proof of "$\implies$"
We can $-1 \equiv \square \bmod p \implies p=x^2+y^2$ in $\mathbb{Z}$ using $\mathbb{Z}[i]$
$$
\begin{align*}
-1 \equiv \square \bmod p &\implies -1 \equiv m^2 \bmod p\\
&\implies p \mid (m^2+1) \text{ in } \mathbb{Z} \subset \mathbb{Z}[i]\\
&\implies p \mid (m+i)(m-i) \text{ in } \mathbb{Z}[i]
\end{align*}
$$
Let's show from this relation that $p$ is composite in $\mathbb{Z}[i]$.Since $p$ is prime or composite in $\mathbb{Z}[i]$, we will show $p$ is *not* prime in $\mathbb{Z}[i]$, by contradiction.

If $p$ were prime in $\mathbb{Z}[i]$, then 
$$
p\mid (m+i)(m-i) \text{ in } \mathbb{Z}[i] \implies p \mid (m+i) \text{ or } p \mid (m-i) \text{ in } \mathbb{Z}[i]
$$
Then either $p(a+bi) = m+i$ or $p(a+bi)=m-i$ for some $a,b \in \mathbb{Z}$. Look at the coefficients of $i$: $pb=1$ in $\mathbb{Z}$ or $pb=-1$ in $\mathbb{Z}$. Hence $p$ is not prime in $\mathbb{Z}[i]$, so it's composite.

Thus, $p=\alpha \beta$ for *non-units* $\alpha,\beta \in \mathbb{Z}[i]$. Apply norm to both sides,
$$
p^2 = N(\alpha)N(\beta) \text{ in } \mathbb{Z}
$$
And $N\alpha,N\beta >1$ since $\alpha,\beta \neq$ units and norms $\geq 0$ in $\mathbb{Z}[i]$.

Thus, $N\alpha =p$ and $N\beta = p$. If $N\alpha=p$ then we can write $\alpha = x+yi$, so $p=N\alpha=N(x+yi)=x^2+y^2$. $\qquad \square$

#### Proof of "$\impliedby$"
Both sides true at $p=2$ so let $p>2$.

*Step 1:* $p =x^2+y^2$ in $Z \implies p \not\mid y$.
	Proof #1:
	$$
	\begin{align*}
	y \neq 0, \text{ so } p \mid y &\implies y^2 \geq p^2\\
	&\implies x^2+y^2 \geq p^2\\
	&\implies p>p^2 \text{ (contradiction)}
	\end{align*}
	$$
	Proof #2:
	$$
	\begin{align*}
	p=x^2+y^2 &\implies x^2+y^2 \equiv 0\bmod p\\
	\text{So }p\mid y &\implies x^2 \equiv 0 \bmod p\\
	&\implies x \equiv - \bmod p \text{ ($p$ prime)}\\
	&\implies p\mid x
	\end{align*}
	$$
	$\implies x^2+y^2 \equiv 0 \bmod p$ 
	$\implies p \equiv 0 \bmod p^2$: NO! Thus, $p\not\mid y$
*Step 2:* $p=x^2+y^2$ in $\mathbb{Z}$, $p\not\mid y \implies -1 \equiv \square \bmod p$
$$
\begin{align*}
p=x^2+y^2 &\implies x^2+y^2 \equiv 0 \bmod p\\
&\implies x^2 \equiv -y^2 \bmod p
\end{align*}
$$
By Step 1, $y \not\equiv 0 \bmod p$, so 
$$
\begin{align*}
x^2 \equiv - y^2 \bmod p &\implies (xy^{-1})^2 \equiv -1 \bmod p\\
&\implies -1 \equiv \square \bmod p.
\end{align*}
$$
*Remark:* Some reasoning shows for $d\in \mathbb{Z}$ that $p=x^2-dy^2$ in $\mathbb{Z}$ for prime $p$ $\implies d\equiv \square \bmod p$ (On Set 6: $d=2$)

For $d\in \mathbb{Z}$, $p$ prime, does 
$$
d\equiv \square \bmod p \implies p = x^2-dy^2 \text{ in } \mathbb{Z} \text{ ?}
$$
Yes, if $d=-1$ (using properties of $\mathbb{Z}[i]$). 

Counterexample with $d=3$
	$3\equiv \square \equiv 5^2 \bmod 11$ but $11 \neq x^2-3y^2$ in $\mathbb{Z}$ since $11\not\equiv \square \bmod 3$.
	*Wait:* $-11=x^2-3y^2 = 1^2-3 \cdot 2^2$.

*Fact:* If $\mathbb{Z}[\sqrt{ d }]$ has unique factorization, like $\mathbb{Z}[i]$, the argument used with $\mathbb{Z}[i]$ can be adapted to show $d\equiv \square \bmod p \implies p\text{ or }-p\text{ is } x^2-dy^2\text{ in } \mathbb{Z}$.

Turns out that at $d=2$, we have $-p=x^2-2y^2$ in $\mathbb{Z}$ $\implies p = x'^2-2y'^2$ in $\mathbb{Z}$.

Since $\mathbb{Z}[s\sqrt{ 2 }]$ has unique factorization, we have
$$
\begin{align*}
2 \equiv \square \bmod p &\implies p\text{ or } -p \text{ is } x^2-2y^2\\
&\implies p = x^2 -2y^2\text{ in } \mathbb{Z}
\end{align*}
$$
Thus, 
$$
2\equiv \square \bmod p \iff p =x^2 -2y^2 \text{ in } \mathbb{Z}
$$
