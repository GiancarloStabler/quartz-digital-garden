#theorem #abstract-algebra/ring-theory 

#### Intuition


#### Formal Statement
For $f: R \to S$ a morphism. If we fix $\bar{s} \in S$, then there exists a unique $F: R[x] \to S$ characterized by,
- $F \mid_{R}= f$ ($F$ is equivalent to $f$ when restricted to $R$).
- $F(x)=\bar{s}$.

In fact, $F(a_{0}+a_{1}x+ \ldots + a_{n}x^n)= f(a_{0}) + f(a_{1})\bar{s} + f(a_{2})\bar{s}^2 + \ldots + f(a_{n})\bar{s}^n$. In particular, if $\underset{f=\operatorname{id}_{f}}{R=S}$ and $\bar{r} \in R$, we can evaluate $P(x)$ at $x = \bar{r}$ by $P(\bar{r})=a_{0}+a_{1}\bar{r}+\ldots + a_{n}\bar{r}^n$.

#### Corollaries
- $P(x) \in R[x] \rightsquigarrow \varphi_{p}: R\to R$ given by $\varphi_{p}(r)=P(r)$ polynomial functions. Caution: it can happen that different polynomials have same polynomial function.