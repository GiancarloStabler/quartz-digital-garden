---
dg-publish: true
---
#note #number-theory/quadratic-reciprocity  

[[Quadratic Reciprocity Law]]
#### Main Law
For distinct odd primes $p$ and $q$,
1) If $q\equiv 1 \bmod 4$, then $q\equiv \square \bmod p \iff p\equiv \square \bmod q$.
2) If $q\equiv 3 \bmod 4$, then $-q \equiv \square \bmod p \iff p \equiv \square \bmod q$.

#### Supplementary Law
For odd prime $p$, 
1) $-1\equiv \square \bmod p \iff p \equiv 1 \bmod 4$. ([[Proof of Theorem about Primes as Sums of Squares#Proof of "$ implies$"|related proof]])
2) $2 \equiv \square \bmod p \iff p \equiv 1,7 \bmod 8$.

#### Expressing these Using the [[Legendre Symbol]]

##### Properties
1) $a^{\frac{p-1}{2}} \equiv \left(\frac{a}{p} \right) \bmod p$ for all $a\in\mathbb{Z}$.
2) $\left( \frac{ab}{p}\right) = \left(\frac{a}{p} \right)\left(\frac{b}{p}\right)$ for all $a,b \in \mathbb{Z}$. 

##### Rewrite Quadratic Reciprocity

If $p$ or $q$ is $1 \bmod 4$, then $q \equiv \square \bmod p \iff p \equiv \square \bmod q$.
	$q \equiv \square \bmod p \iff \left( \frac{ q }{ p } \right)$
	$p \equiv \square \bmod q \iff \left( \frac{ p }{ q } \right)$
Thus, if $p$ or$q$ is $1 \bmod 4$, then $\left( \frac{ q }{ p } \right)= \left( \frac{ p }{ q } \right)$.

If $p$ and $q$ are $3 \bmod 4$, then $-q \equiv \square \bmod p \iff p \equiv \square \bmod q$.
	$-q \equiv \square \bmod p \iff \left( \frac{  -q }{ p } \right)$
	$p\equiv \square\bmod q \iff \left( \frac{ p  }{ q } \right)$
Thus, if $p$ and $q$ are $3 \bmod 4$, then 

By multiplicativity of the Legendre symbol, 
	$p$ and $q$ are $3 \bmod 4 \implies \left( \frac{ -q }{ p } \right)= \left( \frac{ -1 }{ p } \right)\left( \frac{ q }{ p } \right) = -\left( \frac{ q }{ p } \right)$ since $-1 \not\equiv \square \bmod p$ when $p \equiv 3 \bmod 4$.

##### New Statement of Main Law 
For odd primes $p\neq q$, 
1) $p$ or $q$ is $1\bmod 4 \implies \left( \frac{ q }{ p } \right) = \left( \frac{ p }{ q } \right)$
2) $p$ or $q$ are $3\bmod 4 \implies \left( \frac{ q }{ p } \right)= - \left( \frac{ p }{ q } \right)$

##### New Statement of Supplementary Laws
For odd primes $p$,
$$
\left( \frac{ -1 }{ p } \right)=\begin{cases}
1 & \text{if } p \equiv 1 \bmod 4 \\
-1 & \text{if } p \equiv 3 \bmod 4 \ [p\not\equiv 1 \bmod 4]
\end{cases}
$$
$$
\left( \frac{ 2 }{ p } \right) = \begin{cases}
1 & \text{if } p \equiv 1,7\bmod 8 \\
-1 & \text{if } p \equiv 3,5 \bmod 8 \ [p\not\equiv 1,7 \bmod 8]
\end{cases}
$$

#### Examples
1) Is $29 \equiv \square \bmod 59$? ($\left( \frac{ 29 }{ 59 } \right)=1$?)
	$29,59$ both primes
	$29 \equiv 1 \bmod 4$
	$\left( \frac{ 29 }{ 59 } \right)=\left( \frac{ 59 }{ 29 } \right)$ by main law since $29\equiv 1 \bmod 4$
	$\left( \frac{ 29 }{ 59 } \right)=\left( \frac{ 1 }{ 29 } \right)$ since $59 \equiv 1 \bmod 29$
	$\left( \frac{ 29 }{ 59 } \right)= 1$ since $1\equiv 1^{2} \bmod 59$
	Yes: $29 \equiv \square \bmod 59$
	Search finds that $29\equiv 18^2\bmod 59$ 
2) Is $31 \equiv \square \bmod 59$? (What is $\left( \frac{ 31 }{ 59 } \right)$?)
	Both are prime and $31 \equiv 3 \bmod 4$ 
	$59 \equiv 3 \bmod 4$
	$\left( \frac{ 31 }{ 59 } \right)= -\left( \frac{ 59 }{ 31 } \right)$ by main law since $31,59\equiv 3 \bmod 4$
	$\left( \frac{ 31 }{ 59 } \right)=-\left( \frac{ 28 }{ 31 } \right)$ since $59\equiv 28 \bmod 31$
	$\left( \frac{ 31 }{ 59 } \right)= -\left( \frac{ 4\cdot7 }{ 31 } \right)$
	$\left( \frac{ 31 }{ 59 } \right)=-\left( \frac{ 4 }{ 31 } \right)\left( \frac{ 7 }{ 31 } \right)$
	$\left( \frac{ 31 }{ 59 } \right)=-\left( \frac{ 7 }{ 31 } \right)$ 
	$\left( \frac{ 31 }{ 59 } \right) =-\left(-\left( \frac{ 31 }{ 7 } \right) \right)$ since $7,31\equiv 3 \bmod 4$
	$\left( \frac{ 31 }{ 59 } \right)=\left( \frac{ 31 }{ 7 } \right)=\left( \frac{ 3 }{ 7 } \right)=-1$ since $3\not\equiv \square \bmod 7$
