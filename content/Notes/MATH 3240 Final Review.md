---
dg-publish: true
---
#number-theory 
#### [[MATH 3240]]

#### Review Session Notes

[[Wilson's Theorem]]


He won't ask us to prove the main law of quadratic reciprocity, nor the supplementary law for $2$. This seems like a hint that another supplementary law will be on there!


We will get a list of squares $\bmod p$ (up to $13$).


##### Theorem Problem 7
For primes $p>3$,
- $\left(  \frac{ 3 }{ p }  \right)=1 \iff p \equiv 1, 11 \bmod 12$.
- $\left(  \frac{ 6 }{ p }  \right)=1 \iff p \equiv 1,5,19,23 \bmod 24$.

Recall the [[Quadratic Reciprocity Law|main law of quadratic reciprocity]]
	$\left(  \frac{ q }{ p }  \right)=(-1)^{\frac{p-1}{2}\frac{q-1}{2}}\left(  \frac{ p }{ q }  \right)$.

So $\left(  \frac{ 3 }{ p }  \right)= (-1)^{\frac{p-1}{2}\frac{3-1}{2}}\left(  \frac{ p }{ 3 }  \right)=(-1)^{\frac{p-1}{2}}\left(  \frac{ p }{ 3 }  \right)$. It is easy to decide when each term is $1$ or $-1$.

$\left(  \frac{ 3 }{ p }  \right)=1 \iff (-1)^{\frac{p-1}{2}}=1,\left(  \frac{ p }{ 3 }  \right)=1$ OR $(-1)^{\frac{p-1}{2}}=-1, \left(  \frac{ p }{ 3 }  \right)=-1$.

In the first case, we have $p\equiv 1\bmod 4$ and $p\equiv 1 \bmod 3$, thus $p\equiv 1 \bmod 12$.

In the second case, we have $p\equiv 3 \bmod 4$ and $p \equiv 2 \bmod 3$, thus $p \equiv 11 \bmod 12$.

Now for $\left(  \frac{ 6 }{ p }  \right)$

$\left(  \frac{ 6 }{ p }  \right) = \left(  \frac{ 2 }{ p }  \right)\left(  \frac{ 3 }{ p }  \right)$


He won't ask us to do work with Bezout's Identity in $\mathbb{Z}[\sqrt{ 2 }]$


Know how to do division algorithm in all the fields we used ($\mathbb{Z}$, $\mathbb{Z}[i]$, $\mathbb{Z}[\sqrt{ d }]$, $\mathbb{F}[x],$ etc)


Understand the proofs on the review sheets, and the ones on the exam should be no issue.


Same with numerical problems.


Know how to determine if there exists a solution to a quadratic congruence.


##### Division Algorithm in
$\mathbb{Z}$: For $a,b\in \mathbb{Z}$ with $b \neq 0$
$\mathbb{Z}[i]$: For $\alpha,\beta \in \mathbb{Z}[i]$, with $N(\beta)\neq 0$, there exists $\gamma,\rho \in \mathbb{Z}[i]$ such that 


Know the main law of quadratic reciprocity as well as the two supplementary laws we covered (-1 and 2).z


Look up in every $\mathbb{Z}[\sqrt{ d }]$ that $N(\alpha)= \pm p$ for prime number $p$ implies that $\alpha$ is prime in $\mathbb{Z}[\sqrt{ d }]$.