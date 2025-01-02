---
dg-publish: true
---
#example #number-theory/quadratic-integers 

Similarly to other 
#### Factor into Primes in $\mathbb{Z}[i]$

$3+4i: N(3+4i)=25=5^2$
Try $1+2i$,
$$
\begin{align*}
\frac{{3+4i}}{1+2i} &= \frac{{(3+4i)(1-2i)}}{(1+2i)(1-2i)},\\
&= \frac{{11-2i}}{5}\not\in \mathbb{Z}[i].
\end{align*}
$$
Try $1-2i$,
$$
\begin{align*}
\frac{{3+4i}}{1-2i} &= \frac{{(3+4i)(1+2i)}}{(1+2i)(1-2i)},\\
&= \frac{{-5+10i}}{5},\\
&= -1+2i \in \mathbb{Z}[i].
\end{align*}
$$
So,
$$
\begin{align*}
3+4i &= (1-2i)(-(1-2i)),\\
&= -(1-2i)^2,\\
&= i^2(1-2i)^2= (i(1-2i))^2,\\
&= (2+i)^2
\end{align*}
$$

#### Multiple Prime Factorization in $\mathbb{Z}[\sqrt{ 2 }]$
$$
17=(5+2\sqrt{ 2 })(5-2\sqrt{ 2 })=(3\sqrt{ 2 }+1)(3\sqrt{ 2 }-1)=(37+26\sqrt{ 2 })(37-26\sqrt{ 2 })
$$
Because we know that unique prime factorization (up to a unit multiple) exists in $\mathbb{Z}[\sqrt{ 2 }]$, let's try,
$$
\frac{{5+2\sqrt{ 2 }}}{3\sqrt{ 2 }+1} = {{5+2\sqrt{ 2 }}}{1+3\sqrt{ 2 }} = \frac{{(5+2\sqrt{ 2 })(1-3\sqrt{ 2 })}}{(1+3\sqrt{ 2 })(1-3\sqrt{ 2 })} \not\in \text{ Units of }\mathbb{Z}[\sqrt{ 2 }].
$$
...some other work... -> $3\sqrt{ 2 } -1$ is a unit multiple of $5+2\sqrt{ 2 }$!

This is all just a result of multiplying a factorization by $u\cdot u^{-1}$ where $u$ is a [[Unit (Ring)|unit]] and then "attaching" each of them to a different factor.


#### Lack of Unique Factorization

There are examples of rings in which unique factorization does not hold. For example, in $\mathbb{Z}[\sqrt{ 5 }]$,
$$
4=2\cdot 2 = (\sqrt{ 5 }+1)(\sqrt{ 5 }-1).
$$
Which are all prime in $\mathbb{Z}\sqrt{ 5 }$.