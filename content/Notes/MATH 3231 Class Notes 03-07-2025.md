#note #abstract-algebra/field-theory 

#### Defined [[Normal Extension]]

#### Recall [[Splitting Field]]

#### Theorem 1
If $[E:k] = d < \infty$, ${^{\textstyle E}\big/_{\textstyle k}}$ normal, then $\exists P(x) \in k[x]$ such that
$$
{^{\textstyle E}\big/_{\textstyle k}}\simeq \operatorname{split}_{k}(P(x)) \quad(\text{{an isomorphism of extensions}}).
$$
##### Proof
$[E:k] = d < \infty \implies \exists \beta_{1},\ldots,\beta_{d}$ a basis for ${^{\textstyle E}\big/_{\textstyle k}}$ as a vector space over $k$.

Let $m_{i}(x) \overset{def}{=} m_{{\beta_{1}/k}}(x)$
$P(x) = \prod_{i=1}^{d}m_{i}(x)$.

Claim ${^{\textstyle E}\big/_{\textstyle k}}$ isa. splitting field for $P(x)$ over $k$.
$\vdots$

#### Theorem 2
If $k$ field, $P(x) \in k[x]$ nonzero, $E = \operatorname{split}_{k}(P(X))$ is a finite normal extension of $k$.

##### Note
Not all $\alpha \in E$ are roots of $P(x)$, so statement is not trivial. Why does $m_{{\alpha/k}}(x)$ necessarily split as a product of $\deg 1$ polynomials in $E[x]$?

```tikz
\usepackage{tikz-cd}

\begin{document}

\begin{tikzcd} && k &&& k \\ 
\\ 
&&&&&&& {\phi(A(\alpha))A(\beta)\ \forall A[x] \in k[x] } 
\\ && {k[\alpha]} &&& {k[\beta]} && {\phi(\alpha)=\beta} 
\\ 
\\ 
E \\ 
&& F &&& F 
\arrow["{\operatorname{id}_k}", tail reversed, from=1-3, to=1-6] 
\arrow[hook, from=1-3, to=4-3] 
\arrow[hook, from=1-6, to=4-6] 
\arrow["\sim", from=4-3, to=4-6] 
\arrow["\circlearrowleft", shift left=5, curve={height=-30pt}, draw=none, from=4-3, to=4-6] 
\arrow["\circlearrowleft"', shift right=5, curve={height=30pt}, draw=none, from=4-3, to=4-6] 
\arrow[hook, from=4-3, to=6-1] 
\arrow[hook, from=4-3, to=7-3] 
\arrow[hook, from=4-6, to=7-6] 
\arrow[hook, from=6-1, to=7-3] 
\arrow["{\exists \varphi \text{ isom.}}", from=7-3, to=7-6] 
\end{tikzcd}

\end{document}
```

#### Remark
We know how to construct many elements of $\operatorname{Gal}({^{\textstyle \operatorname{split}_{k}(P(x))}\big/_{\textstyle k}})$.

##### Example
Compute $\operatorname{Gal}(\operatorname{split}_{\mathbb{Q}}({^{\textstyle (x^3-2)}\big/_{\textstyle \mathbb{Q}}}))$.

_Solution:_
$x^3-2=(x-\sqrt[3]{ 2 })(x-\sqrt[3]{2  }w)(x-\sqrt[3]{ 2 }w^2)$.
If $\varphi \in \operatorname{Gal}(\mathbb{Q}[\sqrt[3]{2}=\alpha, \sqrt[3]{2}w=\alpha_{2}, \sqrt[3]{2}w^2=\alpha_{3}]/\mathbb{Q})$.
$\varphi$ sends $\left\{ \alpha,\alpha_{2},\alpha_{3} \right\}$ to $\left\{ \alpha, \alpha_{2}, \alpha_{3} \right\}$ (sends roots to conjugates).
$\varphi$ injective (automorphism), $\varphi$ permutes $\alpha,\alpha_{2},\alpha_{3}$.
