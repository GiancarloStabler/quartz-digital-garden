---
dg-publish: true
---
#proof #abstract-algebra/group-theory 

[[Theorem - Chinese Remainder Theorem]]
#### Proof
$f:\mathbb{Z}_{n} \to \mathbb{Z}_{a} \times \mathbb{Z}_{b}$
$f(i\bmod n) = (i\bmod a, i \bmod b)$
$f$ is well-defined. If $i\equiv i' \bmod n$, then $i \equiv i' \bmod a, i\equiv i' \bmod b$

$i\equiv i' \bmod n \implies a\cdot b= n \mid i'-i \implies a \mid i'-i,b\mid i'-i \implies i' \equiv i \bmod a, i' \equiv i \bmod b$ 

$f$ is a morphism:
$f(i+j)=(i+j \bmod a, i+j \bmod b)$
$\quad = (i\bmod a, i \bmod b)+(j\bmod a, j \bmod b)$
$\quad = f(i\bmod n) + f(j\bmod n)$

$f$ is injective: 
It is enough to see $\ker f = \{ 0 \bmod n \}$
If $i \bmod n \in \ker f \implies f(i \bmod n) = (0 \bmod a, 0 \bmod b)$
$\implies i \equiv 0 \bmod a \implies a\mid i$
$\implies i =0 \bmod b \implies b \mid i$
$\implies \operatorname{lcm}(a,b) \mid i \implies n \mid i \implies i \equiv - \bmod n$.

$f$ is surjective:
$\mathbb{Z}_{n}$ has $n$ elements
$\mathbb{Z}_{a}$ has $a$ elements
$\mathbb{Z}_{b}$ has $b$ elements 
$\implies \mathbb{Z}_{a}\times \mathbb{Z}_{b}$ has $ab=n$ elements.
*Fact*: if $A,B$ are sets with $n$ elements, and there exists an injective function $f:A\to B$, then it is surjective as well. 

Therefore, $f$ is a bijection, so it is an isomorphism. $\qquad \square$

