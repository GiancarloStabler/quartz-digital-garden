---
dg-publish: true
---
#proof #number-theory/quadratic-reciprocity 

#### Theorem


#### Case 1: $( \frac{ -1 }{ p } )=1$ and $( \frac{ p }{ 5 } )=1$
$(  \frac{ -1 }{ p }  )=1 \iff p \equiv 1 \bmod 4$ by supplementary law for $(  \frac{ -1 }{ p }  )$.
$\left(  \frac{ p }{ 5 }  \right)=1 \iff p \equiv 1,4 \bmod 5$.
$$
\begin{array}{c | c | c}
p \bmod 4 & p \bmod 5 & p \bmod 20 \\
\hline
1 & 1 & 1 \\
1 & 4 & 9
\end{array}
$$
#### Case 2: $( \frac{ -1 }{ p } )=-1$ and $( \frac{ p }{ 5 } )=-1$
$(  \frac{ -1 }{ p }  )=-1 \iff p \equiv 3 \bmod 4$ by supplementary law for $(  \frac{ -1 }{ p }  )$.
$\left(  \frac{ p }{ 5 }  \right)=-1 \iff p \equiv 2,3 \bmod 5$.
$$
\begin{array}{c | c | c}
p \bmod 4 & p \bmod 5 & p \bmod 20 \\
\hline
3 & 2 & 7 \\
3 & 3 & 3
\end{array}
$$

*Note:*
$$
\begin{align*}
\left(  \frac{ 6 }{ p }  \right)&=\left(  \frac{ 2 }{ p }  \right)\left(  \frac{ 3 }{ p }  \right)\\
&= \left(  \frac{ 2 }{ p }  \right)\left( (-1)^{\left( \frac{p-1}{2} \right)\left( \frac{3-1}{2} \right)}\left(  \frac{ p }{ 3 }  \right) \right) \text{ by Main Law}\\
&= \left(  \frac{ 2 }{ p }  \right)(-1)^{\frac{p-1}{2}}\left(  \frac{ p }{ 3 }  \right) \rightarrow 3 \text{ Legendre symbols depending on $p \bmod 8$, and $p \bmod 3$, which is $p \bmod 24$.}
\end{align*}
$$

#### Goal: Prove Quadratic Reciprocity Law

- On Problem Set 1 or 2 we checked each $a\bmod p$ is $x^2+y^2 \bmod p$ ($p=2,\ldots,29$).

*Show:* Each $a \bmod p$ is $x^2+y^2 \bmod p$ for *every* prime $p$ by giving a formula for $\#\{ x^2+y^2\equiv a \bmod p \}$.

- Look at
$$
N_{n,p} = \# \{ (x_{1},\ldots,x_{n}) \bmod p : x_{1}^2+x_{2}^2+\ldots + x_{n}^2 \equiv 1 \bmod p \}
$$
	Find a recursion for $N_{n,p}$ from $N_{n-2,p}$ for $n \geq 3$ by induction on $n$

- For distinct primes $p,q > 2$, we'll calculate $N_{q,p}\bmod p$ in *two* ways and the quadratic reciprocity will fall out.