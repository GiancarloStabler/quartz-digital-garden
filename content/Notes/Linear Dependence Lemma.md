#theorem #abstract-algebra/vector-spaces 

#### Intuition


#### Formal Statement
Suppose $v_{1},\ldots, v_{m}$ is a linearly dependent list in $V$. Then there exists $k \in \{ 1,\ldots,m \}$ such that $v_{k}\in \operatorname{span}(v_{1},\ldots, v_{k-1})$. Moreover, $\operatorname{span}(v_{1},\ldots,v_{k-1},v_{k+1},\ldots, v_{m})=\operatorname{span}(v_{1},\ldots, v_{m})$.

#### Proof
Since the list is linearly dependent, there exist $a_{i}\in \mathbb{F}$ (not all $0$) such that, $0=a_{1}v_{1}+\cdots + a_{m} v_{m}$. Let $k$ be the largest element of $\{  1,\ldots, m \}$ such that $a_{k}\neq 0$.

Then, $v_{k}= -\frac{{a_{1}}}{a_{k}}v_{1}- \cdots - \frac{{a_{k-1}}}{a_{k}}v_{k-1}$, so $v_{k} \in \operatorname{span}(v_{1},\ldots, v_{k-1})$.

Now suppose $k$ is as above. Let $b_{1},\ldots, b_{k-1}\in \mathbb{F}$ be such that $v_{k}=b_{1}v_{1}+ \cdots + b_{k-1}v_{k-1}$. Suppose $u\in \operatorname{span}(v_{1},\ldots,v_{m})$, then $u=c_{1}v_{1}+ \cdots c_{m}v_{m} =(c_{1}+c_{k}b_{1})v_{1}+\cdots + (c_{k-1}+c_{k}b_{k-1})v_{k-1}+ c_{k+1}v_{k+1}+ \cdots + c_{m}v_{m}$, so $u\in \operatorname{span}(v_{1},\ldots, v_{k-1},v_{k+1},\ldots, v_{m})$.


#### Corollaries