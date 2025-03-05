#theorem #abstract-algebra/field-theory

#### Intuition


#### Formal Statement
For a field $k$, and $P(X) = a_{n}x^n+ \cdots + a_{1}x + a_{0} \in K[X]$. If ${^{\textstyle E}\big/_{\textstyle K}}$, ${^{\textstyle F}\big/_{\textstyle K}}$ are splitting fields of $P(X)$ over $k$, then there exists $\varphi: {^{\textstyle E}\big/_{\textstyle k}}\to {^{\textstyle F}\big/_{\textstyle k}}$ an isomorphism of field extensions ($\varphi \mid_{k} = \operatorname{id}_{k}$).

#### Corollaries
1) Up to isomorphism, we can define *the* splitting field of $P(X)$. Denote it $\operatorname{split}_{k}(P(X))$ or $\operatorname{split({^{\textstyle P(X)}\big/_{\textstyle k}})}$.

#### Proof
We prove a slightly stronger statement by induction on $n$:
Claim: If $\phi: k \to K$ an isomorphism of fields and $\Phi: k[X] \to K[X]$ the induced isomorphism given by $\Phi(b_{m}x^m+ \cdots + b_{1}x+b_{0})=\phi(b_{m})x^m+ \cdots + \phi(b_{1})x+\phi(b_{0})$ with $b_{i}\in k$ and $\phi(b_{i}) \in K$.

If ${^{\textstyle E}\big/_{\textstyle k}}$ a splitting field for $P(X)$ over $k$, ${^{\textstyle F}\big/_{\textstyle K}}$ is a splitting field for $\Phi(P(X))$ over $K$, then

```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{math}
\begin{tikzcd} 
k &&& K \\
&&&&& {\varphi \circ i = j \circ \phi} \\
&&&&& {\varphi \mid_k = \phi} \\
E &&& F 
\arrow["{\phi}", from=1-1, to=1-4] 
\arrow["i"', hook, from=1-1, to=4-1] 
\arrow["j", hook, from=1-4, to=4-4] 
\arrow["{\varphi}"', dashed, from=4-1, to=4-4] 
\end{tikzcd}
\end{math}
\end{document}
```

##### Remark
$k=K$, $\varphi=\operatorname{id}_{k}$ is the Theorem.

##### Proof of Claim by Induction on $n=\deg P(x)$
...


#### Remarks
If $k \leq E \leq \operatorname{split}_{k}(P(X))$, then $\operatorname{split_{k}(P(X))}$ is also a splitting field of $P(X)$ over $E$.

