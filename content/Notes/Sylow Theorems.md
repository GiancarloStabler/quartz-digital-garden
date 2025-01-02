---
dg-publish: true
---
#theorem #abstract-algebra/group-theory 
#### Theorem 1
If $|G| = p^n \cdot m$, there exists $H\leq G$ with $|H|=p^n$ for $p\geq 2$ prime, $n\geq 0$, $m\geq 1$.
(Generalizes [[Cauchy's Theorem]])
#### Theorem 2
Every [[p-subgroup]] $H\leq G$ is contained $H\leq P \leq G$, where $P$ is a [[Sylow P-subgroup]]. Every Sylow p-subgroup $P$ has the same size, $p^n$. If $P,P'$ are Sylow p-subgroups, then there exists $g\in G$ such that $P'=gPg^{-1}$.

#### Theorem 3
$n_{p}= \#$ Sylow p-subgroups, then
- $n_{p} \mid m$
- $n_{p}\equiv 1 \bmod p$
- $n_{p} = [G:N_{G}(P)]$ 
	$P$ any Sylow p-subgroup
	$N_{G}(P)=$ [[normalizer]] of $P$ in $G$.

##### Theorem 
Every group with $pq$ elements ($p,q$ prime) is cyclic isomorphic to $( \mathbb{Z}_{pq}, + )$.

###### Proof
Cauchy's theorem implies there exists $x\in G$ such that $\operatorname{ord}_{}(x)=p$, and $y\in G$ such that $\operatorname{ord}_{}(y)=q$.

$H=\langle x \rangle$ and $K=\langle y \rangle$.

$H\cap K \leq H$, $H\cap K \leq K$ so by Lagrange's theorem,$|H\cap K| \mid |H| = p$, and $|H\cap K| \mid |K| =q$, so $|H\cap K| =1$ and $H\cap K = \{  e \}$. 

*Claim:* $H,K$ are normal in $G$.
	$p\mid pq$, $p<q \implies p\neq q$, so $p^2 \not\mid pq$.
	Thus, $H$ is a Sylow $p$-subgroup, and $K$ is a Sylow $q$-subgroup.

Theorem 2 implies $n_{p}=\#$ conjugates of $P$ in $G$, $P\unlhd G \iff n_{p}=1$.
We want $n_{p}=n_{q}=1$.

$n_{p}\mid q \overset{q \text{ prime}}{\implies} n_{p}=1$ or $n_{p}=q$, and $n_{p} \equiv 1 \bmod p$, so by assumption $q\not\equiv 1 \bmod p$, we have that $n_{p}=1 \implies H$ (Sylow p-subgroup) is normal.

$n_{q}\mid p \overset{p\text{ prime}}{\implies} n_{q}=1$ or $n_{q}=p$, and $n_{q}\equiv 1 \bmod q$,

...