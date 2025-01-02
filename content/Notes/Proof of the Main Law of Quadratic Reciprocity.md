---
dg-publish: true
---
#proof #number-theory/quadratic-reciprocity 

#### Main Law
For distinct odd primes $p$ and $q$, 
$$
\begin{align*}
\left(  \frac{ q }{ p }  \right) &= \begin{cases}
\left(  \frac{ p }{ q }  \right) & \text{ if $p$ or $q$ is $1 \bmod 4$}\\
-\left(  \frac{ p }{ q }  \right) & \text{ if $p$ and $q$ is $3 \bmod 4$}
\end{cases}\\
&= (-1)^{\frac{p-1}{2}\frac{q-1}{2}}\left(  \frac{ p }{ q }  \right).
\end{align*}

$$

#### Proof
Try to count $\# \{ (x_{1},\ldots, x_{n}) \in \mathbb{Z}/p : x_{1}^2 + \ldots + x_{n}^2 \equiv 1 \bmod p \}$ 
###### $n=1$ 
$\# \{ x \bmod p :x^2 \equiv 1 \bmod p \} = 2$
###### $n=2$
$\# \{ (x,y) \bmod p : x^2 +y^2 \equiv 1 \bmod p \}=\ ??$

$$
\begin{array}{c | c c c c c c c c c c c}
p & 3 & 5 & 7 & 11 & 13 & 17 & 19 & 23 & 29 & 31 & 37\\
\hline
\text{count} & 4 & 4 & 8 & 12 & 12 & 16 & 20 & 24 & 28 & 32 & 36 \\
\end{array}
$$
$\text{count} \rightarrow p \pm 1$
$p+1:3,7,11,19,23,31$
$p-1:5,13,17,29,37$

##### Theorem (Stronger)
For $c \not\equiv 0 \bmod p$, $\# \{  (x,y) \bmod p : x^2 + y^2 \equiv c \bmod p \}$ is independent of $c$ and in fact is $p-\left(  \frac{ -1 }{ p }  \right)$. 
###### Proof 
Observe that $\# \{ x \bmod p : x^2 \equiv c \bmod p \}= 1+ \left(  \frac{ c }{ p }  \right)$. So using this,
$$
\begin{align*}
\# \{ (x,y) \bmod p : x^2 +y^2\equiv c \bmod p \} &= \sum_{\underset{a+b \equiv c \bmod p}{(a,b) \bmod p}}^{} \# \{ x^2 \equiv a \bmod p \} \cdot \{ y^2 \equiv b \bmod p \}\\
&= \sum_{a+b \equiv c \bmod p}^{}\left( 1+\left(  \frac{ a }{ p }  \right) \right) \cdot \left( 1 + \left(  \frac{ b }{ p }  \right) \right)\\
&= \sum_{a+b \equiv c \bmod p}^{} \left( 1+\left(  \frac{ a }{ p }  \right) +\left(  \frac{ b }{ p }  \right)+ \left(  \frac{ ab }{ p }  \right)\right)\\
&= \sum_{a \bmod p}^{} \left( 1+\left(  \frac{ a }{ p }  \right) + \left(  \frac{ c-a }{ p }  \right) + \left(  \frac{ a(c-a) }{ p }  \right) \right)\\
&= \sum_{a}^{}1 + \sum_{a}^{}\left(  \frac{ a }{ p }  \right) + \sum_{a}^{} \left(  \frac{ c-a }{ p }  \right) + \sum_{a}^{} \left(  \frac{ a(c-a) }{ p }  \right)\\
&=\sum_{a}^{}1 + 0 + 0 + \sum_{a}^{} \left(  \frac{ a(c-a) }{ p }  \right)\\
&= p+\sum_{a \bmod p}^{} \left(  \frac{ a(c-a) }{ p }  \right) \rightarrow \text{ indep. of $c$ if $c \not\equiv 0 \bmod p$??}\\
&= p + \sum_{a \bmod p}^{} \left(  \frac{ ca(c-ca) }{ p }  \right) \text{ change of variables $a\rightarrow ca \bmod p$ for $c \not\equiv 0 \bmod p$}\\
&= p + \sum_{a\bmod p}^{} \left(  \frac{ c^2a(1-a) }{ p }  \right)\\
&=v p + \sum_{a\bmod p}^{} \left(  \frac{ c^2 }{ p }  \right)\left(  \frac{ a(1-a) }{ p }  \right), c\not\equiv 0 \bmod p\\
&= p + \sum_{a\bmod p}^{}\left(  \frac{ a(1-a) }{ p }  \right) \rightarrow \text{ indep. of $c$}.
\end{align*}
$$

Why is it $p-\left(  \frac{ -1 }{ p }  \right)$?

Let $N(c) = \# \{  (x,y) \bmod p : x^2 + y^2 \equiv c \bmod p \}$,
So $N(0) + N(1) + N(2) + \ldots + N(p-1) = p^2$ 
	Note that $N(1),N(2),\ldots,N(p-1)$ all have same value.
Thus $N(0) + (p-1)N(1) = p^2$
$\implies N(1) = \frac{p^2 - N(0)}{p-1}, N(0) = \# \{ (x,y) \bmod p : x^2 +y^2 \equiv 0 \bmod p \}$

Note: $x^2+y^2 \equiv 0 \bmod p \implies x^2 \equiv -y^2 \bmod p$, so if $y \not\equiv 0 \bmod p$ then $(x y^{-1})^2 \equiv -1\bmod p$.

- So if $\left(  \frac{ -1 }{ p }  \right) = -1$ ($p\equiv 3 \bmod 4$) then the only solution to $x^2 + y^2 \equiv 0 \bmod p$ is $(0,0) \bmod p : y \equiv 0 \implies x\equiv 0$. Then $N(1) = \frac{p^2-1}{p-1}=p+1$. $\star$
- If $\left(  \frac{ -1 }{ p }  \right)= 1$, write $-1\equiv t^2 \bmod p$. Then $x^2+y^2 \equiv 0 \bmod p \iff x^2 \equiv -y^2 \bmod p \iff x^2 \equiv (ty)^2 \bmod p \iff x\equiv \pm ty \bmod p$. Therefore, $\{ (x,y) : x^2+y^2 \equiv 0 \bmod p \} = \{ (\pm ty,y) : y\in \mathbb{Z}/p \}$, so $\left(  \frac{ -1 }{ p }  \right)=1 \implies N(0) = 1 + 2(p-1)=2p-1 \implies N(1) = \frac{p^2-(2p-1)}{p-1} = \frac{p^2-2p+1}{p-1} = \frac{(p-1)^2}{p-1}=p-1$. $\star$

###### Remark
Knowing $\# \{ (x,y) : x^2+y^2 \equiv 1\bmod p \} = p- \left(  \frac{ -1 }{ p }  \right)$, on LHS, most solutions come in packets of size 8:
$(x,y),(-x,y),(x,-y),(-x,-y),(y,x),(-y,x),(y,-x),(-y,-x) \bmod p$ which are distinct unless $x\equiv 0 \bmod p$, $y\equiv 0 \bmod p$, or $x\equiv y \bmod p$. By counting $N(1) \bmod 8$ we can derive formula for $\left(  \frac{ 2 }{ p }  \right) \rightarrow$ see Thm 3.1 .

...