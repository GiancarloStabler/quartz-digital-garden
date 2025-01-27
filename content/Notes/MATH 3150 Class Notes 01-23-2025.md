#note #analysis/real-analysis 

Today we will focus on $\mathbb{Z}$, $\mathbb{Q}$. We will introduce $\frac{n}{m}$ for $n,m \in \mathbb{Z}$ in an axiomatic way.

#### Properties (Axioms)
1) Addition
	1) $(x+y)+z = x+(y+z)$ associativity for all $x,y,z$.
	2) $x+y=y+x$ commutativity for all $x,y$.
	3) $\exists 0$ such that $x+0=0+x=x$ for all $x$.
	4) $\forall x, \exists (-x)$ such that $x+(-x)=(-x)+x=0$.
2) Multiplication
	1) $(x\cdot y) \cdot z = x \cdot (y \cdot z)$.
	2) $x \cdot y = y \cdot x$.
	3) $\exists 1$ such that $x \cdot 1= 1 \cdot x= x$ for all $x$.
	4) $\forall x \neq 0$, $\exists x ^{-1}$ such that $x \cdot x ^{-1} = x ^{-1} \cdot x = 1$.
3) Distributivity
	1) $x \cdot (y + z) = x \cdot y + x \cdot z$ for all $x,y,z$.

##### Remark
All known properties of rational (or real) numbers follow from these 9 axioms. 

#### Ordering "$\leq$"
1) $\forall x,y$ either $x \leq y$ or $y \leq x$.
2) $\forall x,y$ if $x \leq y$ and $y \leq x$ then $x=y$.
3) If $x \leq y$ and $y \leq z$, then $x \leq z$.
4) If $x \leq y$ then $x+z \leq y+z$.
5) If $x\leq y$ and $0 \leq z$, then $x \cdot z \leq y \cdot z$.

##### Example
$0< 1$ follows from Ordering axioms 1-5 (O1-O5).

###### Proof
$0\neq 1 \overset{O1}{\implies}$ either $0 \leq 1$ or $1 \leq 0$.

Assume for the sake of contradiction that $1 \leq 0$, then by $O4$, $1+(-1)\leq 0 + (-1) \leq -1$. From that we have that $0 \leq -1$, by which we can multiply both sides by $-1$, since we have that $0\leq -1$, we have that $(0)\cdot(-1) \leq (-1)\cdot (-1)$, or $0 \leq 1$, a contradiction.
