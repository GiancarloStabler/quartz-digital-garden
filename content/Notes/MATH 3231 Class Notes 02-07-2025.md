#note #abstract-algebra/ring-theory 

####  [[Prime Ideal|Prime Ideals]]

##### Recall 
$P \unlhd R$ is prime if $xy \in P \implies x$ or $y \in P$ (and $P \neq R$).

##### Remark
$f: R \to S$ morphism and $q \unlhd S$ prime ideal, then $f ^{-1} q \unlhd R$ is a prime ideal.

###### Proof
$x,y \in R$, and $x \cdot y \in f ^{-1} q \implies f(x)f(y) = f(xy) \in q$. 


##### Remark
If $I \unlhd R$ and $I \subseteq P \unlhd R$, with $P$ a prime ideal, then ${^{\textstyle  P}\big/_{\textstyle I}}\unlhd {^{\textstyle R}\big/_{\textstyle I}}$ is prime.

###### Proof
If $x+I, y+I \in {^{\textstyle R}\big/_{\textstyle I}}$ (where $x,y\in R$), $(x+I)(y + I)=(xy+I) \in {^{\textstyle  P}\big/_{\textstyle I}}$, then $xy+I=z+I$ for some $z\in P$, so $xy = \underset{\in P}{z} + \underset{\in I \subseteq P}{t}, t\in I$. Hence $x$ or $y$ are in $P$, so $x+I$ or $y+I$ are in $P$.

##### Corollary: [[Correspondence Theorem for Quotients]]

#### Defined [[Domain]]

##### Remark
If $u\in R$ is a unit ($u$ has a multiplicative inverse in $R$), then $u$ is not a zero-divisor.

###### Proof
$\varphi: R\to R$ defined by $\varphi(x) = ux$. $u$ is a unit $\iff$ $\varphi$ is bijective $\implies$ $\varphi$ injective $\iff$ $u$ is not a zero-divisor.

#### Defined [[Field]]


