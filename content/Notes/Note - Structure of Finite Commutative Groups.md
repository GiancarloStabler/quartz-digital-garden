---
dg-publish: true
---
#note #abstract-algebra/group-theory 

### Isomorphism Classes of Finite Commutative Groups

### Theorem
Let $( G, \cdot )$ be a [[Abelian Group|commutative group]] with $n$ elements, then there exist unique integers $1 < d_{m} \mid d_{m-1} \mid d_{m-2} \mid \ldots \mid d_{1}$ such that $n = d_1 \cdot d_m$ and $G \simeq \mathbb{Z}_{d_{1}} \times \mathbb{Z}_{d_{2}} \times \ldots \times \mathbb{Z}_{d_{m}}$

#### Example 1
List the [[Isomorphism|isomorphism]] classes of finite commutative groups with 6 elements.

$6=d_{1} \cdot \ldots \cdot d_{m}$
$d_{m} \geq 2$
$d_{m}\mid d_{m-1}, d_{m-1}\mid d_{m-2}, \ldots, d_{2} \mid d_{1}$

$6=6 = 2\cdot 3$ but $3 \not\mid 2$.

Therefore by the theorem above, every finite commutative group with 6 elements is [[Cyclic Group|cyclic]] of order $6$ (isomorphic to $\mathbb{Z}_{6}$) 


#### Question
How about $\mathbb{Z}_{2} \times \mathbb{Z}_{3}$? 

*Answer:* We found [[Proof of Chinese Remainder Theorem (Group Theory)|last time]] that $\mathbb{Z}_{2} \times \mathbb{Z}_{3} \simeq \mathbb{Z}_{6}$, because $\gcd(2,3)=1$ and recall the Chinese Remainder Theorem: if $n=ab$, $\gcd(a,b)=1$, then $\mathbb{Z}_{a}\times \mathbb{Z}_{b}\simeq \mathbb{Z}_{n}$.


#### Example 2
List isomorphism classes of commutative groups with 8 elements.

We want to decompose $8=d_{1}\cdot\ldots\cdot d_{m}$ with $d_{m}\geq 2$, $d_{m}\mid d_{m -1} , \ldots , d_{2} \mid d_{1}$, and in particular $d_{1 } \geq d_{2} \geq \ldots \geq d_{m}\geq 2$.

The only ways to write 8 as products of integers in weakly decreasing order is,
1) $8=8$
2) $8=4\cdot 2$
3) $8 = 2 \cdot 2 \cdot 2$

Thus, by the theorem, if $( G, \cdot )$ is commutative with 8 elements, $G \simeq \mathbb{Z}_{8}$, or $\mathbb{Z}_{4}\times \mathbb{Z}_{2}$, or $\mathbb{Z}_{2}\times \mathbb{Z}_{2} \times \mathbb{Z}_{2}$

Note that $\mathbb{Z}_{2}\times \mathbb{Z}_{4} \simeq \mathbb{Z}_{4}\times \mathbb{Z}_{2}$. 

#### Example 3
$( U(16), \cdot )=\{ i\in \mathbb{Z}_{16} : \gcd(i,1)=1 \}$ (this is equivalent to $i$ odd)
$= \{ 1,3,5,7,9,11,13,15 \}$ (note this has 8 elements)

So this is isomorphic to one of those we listed previously, in particular it is isomorphic to $\mathbb{Z}_{4}\times \mathbb{Z}_{2}$.

*Why?*
If not, then it is isomorphic to $\mathbb{Z}_{8}$ or $\mathbb{Z}_{2}\times \mathbb{Z}_{2} \times \mathbb{Z}_{2}$.

If the latter is true, then $i^2\equiv 1$ for all $i\in U(16)$ but $3^2 = 9 \not\equiv 1 \bmod 16$, we have a contradiction.

Otherwise, we check $i^4=1$ for all $i$, so there is no element of order 8, so $U(16)$ is not cyclic.
	$1^4 = 1 \equiv 1 \bmod 16$
	$(-1)^4 =(-1)^4 \cdot 1^4=1\cdot 1^4 = 1$.
	If $i^4. \equiv 1 \bmod 16$ then $(16-i)^4=(-i)^4 \equiv 1 \bmod 16$
	$\implies 15^4 =(-1)^4\equiv 1 \bmod 16$.
	
	$3^4 = 81 =80 + 1 = 16*5 +1 \equiv 1 \bmod 16$
	$\implies 1 \equiv (-3)^4=13^4$
	
	$5^4 = 25^2 \equiv 9^2 = 81 \equiv 1 \bmod 16$
	$\implies 1 \equiv (-5)^4 \equiv 11^4 \bmod 16$
	
	$9^2=81\equiv 1 \bmod 16 \implies 9^4 \equiv 1^2 \equiv 1 \bmod 16$
	$\implies 1 \equiv (-9)^4\equiv 7^4$

#### Example 4
List isomorphism classes of commutative groups with 120 elements.

*Solution:* 
$120=d_{1},d_{2},\ldots,d_{m}$
with $d_{1}\geq d_{2} \geq \ldots \geq d_{m} \geq 2$
and $d_{m} \mid d_{m-1}$, $d_{m-1} \mid d_{m-2}$, etc.

$120=12\cdot 10 = 2^2 \cdot 3 \cdot 2 \cdot 5 = 2^3 \cdot 3 \cdot 5$

The divisibility conditions force $2\cdot 3 \cdot 5=30 \mid d_{1}$
	Options are:
		$120=120$
		$120 = 60 \cdot 2$
		$120 = 30 \cdot 2 \cdot 2$

Then every commutative group with 120 elements is isomorphic to exactly one of $\mathbb{Z}_{120}$, $\mathbb{Z}_{60}\times \mathbb{Z}_{2}$, or $\mathbb{Z}_{30} \times \mathbb{Z}_{2}\times \mathbb{Z}_{2}$.

#### Example 5
$\mathbb{Z}_{12}\times \mathbb{Z}_{10}$ is isomorphic to exactly one on the above list. 

$12=4\cdot 3 \implies \mathbb{Z}_{12}\simeq \mathbb{Z}_{4 }\times \mathbb{Z}_{3}$
$10 = 5 \cdot 2 \implies \mathbb{Z}_{10} \simeq \mathbb{Z}_{5}\times \mathbb{Z}_{2}$

$\mathbb{Z}_{12}\times \mathbb{Z}_{10} \simeq \mathbb{Z}_{4}\times \mathbb{Z}_{3} \times \mathbb{Z}_{5}\times \mathbb{Z}_{2}$ (note that 4,3,5 are pairwise coprime)

By the Chinese Remainder Theorem, $\mathbb{Z}_{4}\times \mathbb{Z}_{3}\times \mathbb{Z}_{5} \simeq \mathbb{Z}_{60}$

Thus, we have that $\mathbb{Z}_{12}\times \mathbb{Z}_{10}\simeq \mathbb{Z}_{60}\times \mathbb{Z}_{2}$. 


#### Proof of Uniqueness

If $G \simeq \mathbb{Z}_{d_{1}} \times \ldots \times \mathbb{Z}_{d_{m}}$ and $G \simeq \mathbb{Z}_{f_{1}} \times \ldots \times \mathbb{Z}_{f_{m}}$

We have,
$d_{1}\geq d_{2} \geq \ldots \geq d_{m} \geq 2$ with $m\geq 1$
$f_{1}\geq f_{2} \geq \ldots \geq f_{r} \geq 2$ with $r \geq 1$

$d_{m} \mid d_{m-1}$, $d_{m-1} \mid d_{m-2}$, etc.
$f_{r} \mid f_{r-1}$, $f_{r-1} \mid f_{r-2}$, etc.

We want that $r=m$ and $d_{i}=f_{i}$ for all $i$.

*Observation:* 
$d_{1}=$ smallest $\{ u\geq 1 : g^u=e_{G} \quad \forall g\in  G \}$
$\vdots$


#### Example 6
We saw that we have $\mathbb{Z}_{120}$, $\mathbb{Z}_{60}\times \mathbb{Z}_{2}$, and $\mathbb{Z}_{30}\times \mathbb{Z}_{2}\times \mathbb{Z}_{2}$ are the only isomorphism classes of commutative groups with 120 elements. These all have different [[Exponent (of a Group)|exponents]] (120, 60, and 30, respectively) which means they are not isomorphic. 

#### Example 7
Every finite commutative group with 16 elements is isomorphic to either $\mathbb{Z}_{16}$, $\mathbb{Z}_{8}\times \mathbb{Z}_{2}$, $\mathbb{Z}_{4}\times \mathbb{Z}_{4}$, $\mathbb{Z}_{4}\times \mathbb{Z}_{2}\times \mathbb{Z}_{2}$, or $\mathbb{Z}_{2}\times \mathbb{Z}_{2}\times \mathbb{Z}_{2}\times \mathbb{Z}_{2}$. 

The exponents of each of these are respectively, 16, 8, 4, 4, and 2. Note that $\mathbb{Z}_{4}\times \mathbb{Z}_{4}$ and $\mathbb{Z}_{4}\times \mathbb{Z}_{2}\times \mathbb{Z}_{2}$ have the same exponent.

How many elements of order 4 do they each have?

In $\mathbb{Z}_{4}\times \mathbb{Z}_{4}$,
	$(1,i),(3,i),(i,1),(i,3)$ have order 4 for any $i\in \mathbb{Z}_{4}$. 
	Excluding repetitions, this leaves us with 12 such elements.
In $\mathbb{Z}_{4}\times \mathbb{Z}_{2}\times \mathbb{Z}_{2}$
	$(1,i,j),(3,i,j)$ have order 4 for any $i,j \in \mathbb{Z}_{2}$.
	This leaves us with 8 such elements.

Thus, we have that $\mathbb{Z}_{4}\times \mathbb{Z}_{4}$ and $\mathbb{Z}_{4}\times \mathbb{Z}_{2}\times \mathbb{Z}_{2}$ are not isomorphic.


#### Proof of Existence

$G \simeq \mathbb{Z}_{d_{1}}\times \ldots \times \mathbb{Z}_{d_{m}}$

*First Step:* We break $G$ into simpler parts.

$n=p_{1}^{\alpha_{1}}\cdot \ldots \cdot p_{r}^{\alpha_{r}}$ where $p_{1}, \ldots p_{r}$ are distinct primes, $\alpha_{i}\geq 1$ for all $i$.

Using the fact from ([[P-Torsion Subgroup]]) that $g,g' \in G[p] \implies \operatorname{ord}_{}(g)=p^k$, $\operatorname{ord}_{}(g')=p^{k'}$ for some $k,k'\in \mathbb{N} \implies \operatorname{ord}_{}(gg')\mid \operatorname{lcm}(p^k,p^{k'})=\operatorname{max}(k,k') \implies \operatorname{ord}_{}(gg')=p^{k''}$ for some $k'' \leq \operatorname{max}(k,k') \implies G[p]$ is stable under products.

(b) Assume $p \mid |G| \overset{ \text{Cauchy} }{\implies} \exists g\in G, \operatorname{ord}_{}(g)=p=p^1 \implies e\neq g\in G[p] \implies G[p] \neq \{ e \}$.

Conversely, if $G[p] \neq \{  e \} \implies \exists e\neq g\in G[p] \implies \operatorname{ord}_{}(g)=p^k$ for some $k>0 \overset{\text{Lagrange}}{\implies}p^k \mid |G| \implies p \mid |G|.$


Next time we show $G \simeq G[p_{1}] \times \ldots \times G[p_{r}]$.

#### Show $G \simeq G[p_{1}] \times \ldots \times G[p_{r}]$

Define $\varphi:G[p_{1}]\times \ldots\times G[p_{r}] \to G$
$p_{1},\ldots,p_{r}$ are the distinct prime factors of $n=|G|$.
$\varphi(a_{1},\ldots,a_{r})=a_{1}\bullet \ldots \bullet a_{r}$

Because $G$ is commutative, we have easily that $G$ is a morphism.

Assume $(a_{1},\ldots,a_{r})\in \ker \varphi$. 
$\implies a_{1}\cdot\ldots\cdot a_{r}=e_{G} \implies a_{1}=a_{2}^{-1}\cdot a_{3}^{-1} \cdot \ldots \cdot a_{r}^{-1}$.

Let $\operatorname{ord}_{}(a_{i}) = p_{i}^{k_{i}}$ for $k_{i}\geq 0$
$\implies \operatorname{ord}_{}((a_{i}^{-1}))= \operatorname{ord}_{}(a_{i})=p_{i}^{k_{i}}$

$p_{1}^{k_{1}}=\operatorname{ord}_{}(a_{2}^{-1}\cdot\ldots\cdot a_{r}^{k_{r}}) =$ divisor of $\operatorname{lcm}(\operatorname{ord}_{}(a_{2}^{-1}),\operatorname{ord}_{}(a_{r}^{-1}))$ since $a_{i}$ commute, this is a divisor of $p_{2}^{k_{2}},p_{r}^{k_{r}}$
$\implies p_{1}^{k_{1}}= 1 \implies k_{1} = 0$, so $a_{1}=e_{G}$.

An inductive argument implies that $a_{i}=e_{G}$ for all $i$, which implies $\ker \varphi = \{ e_{G},\ldots, e_{G} \}$, thus $\varphi$ is injective.


Now show $\varphi$ is surjective.
Let $g\in G$ where $|G|=n$. By [[Theorem|Lagrange's theorem]], we have that $g^n=e_{G}$

$n=p_{1}^{\alpha_{1}}\cdot\ldots \cdot p_{r}^{\alpha_{r}}$ which are $r$ pairwise coprime factors.

By the [[Theorem - Chinese Remainder Theorem|Chinese Remainder Theorem]], $\mathbb{Z}_{n} \underset{\underset{\psi \text{ isomorphism}}{\leftarrow}}{\simeq} \mathbb{Z}_{p_{1}}^{\alpha_{1}}\times \ldots \times \mathbb{Z}_{{p_{r}}}^{\alpha_{r}}$ 
$$
\begin{align*}
p_{1}&= \psi(1,0,\ldots,0)\\
&\vdots \\
p_{r} &= \psi(0,0,\ldots,0,1)
\end{align*}
$$ Note, the $p_{i}$ above could be a $\beta_{i}$...
(Missed some lines that reach the below)

In $\mathbb{Z}\implies \gamma_{1}\beta_{1} + \ldots + \gamma_{r}\beta_{r}=1 \bmod n \implies \gamma_{1}\beta_{1} + \ldots +\gamma_{r}\beta_{r}=1+nk$ for some $k\in \mathbb{Z}$.

$g=g^{-1}$ and $g^n = e$ $\implies g=g^{1+nk} = g^{\gamma_{1}\beta_{1}+\ldots + \gamma_{r} \beta_{r}}= g^{\gamma_{1}\beta_{1}}\cdot\ldots \cdot g^{\gamma_{r}\beta_{r}}$

*Question:* What is the order of $g^{\beta_{1}}$?
$(1,0,\ldots,0) \in \mathbb{Z}_{p_{2}}\alpha_{1}\times \ldots \times \mathbb{Z}_{p_{r}}\alpha_{r}$ has order $p_{1}^{\alpha_{1}} \implies \beta_{1}\in \mathbb{Z}_{n}$ also has order $p_{1}^{\alpha_{1}} \bmod n$.

$\implies p_{1}^{\alpha_{1}} \cdot \beta_{1} \equiv 0 \bmod n$. 
	$\beta_{1}=n\cdot s$ for some $s\in \mathbb{Z}$
$\implies (g^{{\beta_{1}}})^{p_{1}^{\alpha_{1}}}$

From remark in [[Proof of P-group Theorem]],
$G \simeq G[p_{1}] \times\ldots \times G[p_{r}]$

We can use the Chinese Remainder Theorem to regroup as $\mathbb{Z}_{d_{1}}\times \ldots \times \mathbb{Z}_{d_{m}}$, with $d_{m}\mid d_{m-1}\mid\ldots\mid d_{2}\mid d_{1}$ and $d_{1}\cdot \ldots \cdot d_{m} = p$.


#### Example 
Say $G=G[2] \times G[3] \times G[5]$
which respectively are $\mathbb{Z}_{4}\times \mathbb{Z}_{2}, \mathbb{Z}_{9}\times \mathbb{Z}_{9} \times \mathbb{Z}_{3},\mathbb{Z}_{5}\times \mathbb{Z}_{5}$.

Arrange the indices as

In columns $4,9,5$ are pairwise coprime, as are $2,9,5$, and $1,3,1$.

Thus, by the Chinese Remainder Theorem
	$\mathbb{Z}_{4}\times \mathbb{Z}_{9}\times \mathbb{Z}_{5} \simeq \mathbb{Z}_{4\cdot{9}\cdot{5}} = \mathbb{Z}_{180}$
	$\mathbb{Z}_{}$