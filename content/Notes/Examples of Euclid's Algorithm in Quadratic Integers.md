---
dg-publish: true
---
#example #number-theory/quadratic-integers 

### Example of Euclid's Algorithm in $\mathbb{Z}[i]$

$\alpha= 4+5i$ : $N(\alpha) = 16+25 = 41$
$\beta=4-5i$ : $N(\beta) = 16+25 = 41$

Thus, $\alpha,\beta$ are primes in $\mathbb{Z}[i]$.

$$
\begin{align*}
4+5i &= (4-5i)(i) + (-1+i)\\
4-5i &= (-1+i)(-5) - 1\\
-1+i &= (-1)(1-i) + 0
\end{align*}
$$
$GCD = -1$ (a unit!)

Use Euclid's algorithm to write $(4+5i)x+(4-5i)y=1$ in $\mathbb{Z}[i]$:

$$
\begin{align*}
-1 &= (4-5i)-(-1+i)(-5),\\
&= (4-5i)+(-1+i)5,\\
&= (4-5i)(4+5i - (4-5i)i)5,\\
&= (4-5i) + (4+5i)5 +(4-5i)(-5i),\\
&= (4+5i)5+(4-5i)(1-5i),\\
1 &= (4+5i)(-5) + (4-5i)(-1+5i).
\end{align*}
$$
$$
x=-5, y=(-1+5i)
$$

